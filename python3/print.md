# print()

### 기본
__1.__
```python
print('Hello World')
```
```
Hello World
```

__2.__
```python
print('Hello', 'World')
```
```
Hello World
```

__3.__
```python
x = 1
y = 1
print(x, y, x + y)
```
```
1 1 2
```

<br>
작은따옴표 대신 큰따옴표도 쓸 수 있다. 두 개의 차이점은 없다.

```python
print("Hello World")
```
```
Hello World
```

<br>
큰따옴표 안에 작은따옴표를 넣을 수 있고, 그 반대도 가능하다.

```python
print("'Hello World'")
```
```
'Hello World'
```

<br>

```python
print('"Hello World"')
```
```
"Hello World"
```

***

### 옵션

__1. `sep`__

`sep`를 쓰지 않으면 공백으로 설정된다.  
```python
print('Hello', 'World')
```
```
Hello World
```

<br>
작은따옴표 안에 문자나 문자열을 넣을 수 있다.

```python
print('Hello', 'World', sep='@')
```
```
Hello@World
```

<br>
작은따옴표 안에 아무것도 넣지 않으면 붙어서 출력된다.

```python
print('Hello', 'World', sep='')
```
```
HelloWorld
```

<br>

__2. `end`__

`end`를 쓰지 않으면 줄바꿈 문자(\n)으로 설정된다.

```python
print('Hello World')
print('Python3')
```
```
Hello World
Python3
```

<br>
작은따옴표 안에 문자나 문자열을 넣을 수 있다.

```python
print('Hello World', end='#')
print('Python3')
```
```
Hello World#Python3
```

<br>
작은따옴표 안에 아무것도 넣지 않으면 붙어서 출력된다.

```python
print('Hello World', end='')
print('Python3')
```
```
Hello WorldPython3
```

***

### 기타

__1.__ `sep`과 `end`를 같이 사용할 수 있다.

```python
print('Hello', 'World', sep=', ', end='...')
print('Python3')
```
```
Hello, World...Python3
```
***
