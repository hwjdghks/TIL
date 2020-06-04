# input()

### 기본

```python
var = input()    # 키보드로 입력받은 값을 문자열로 var에 저장한다
```

<br>

```python
var = input()
print(var)
```
```
Hello World!    # Hello World! 입력
Hello World!
```

<br>
()안에 출력할 값을 설정할 수 있다.

```python
var = input('input: ')
```
```
input:     # 입력 대기 상태
```

***

### 메소드

> split()

공백을 기준으로 값을 나눠서 저장할 수 있다.

```python
var1, var2 = input('input: ').split()
print(var1)
```
```
input: Hello World!    # Hello World! 입력
Hello                  # var1 = 'Hello', var2 = 'World!'
```

<br>
()안에 공백 대신 사용할 구분자를 입력할 수 있다.

```python
var1, var2 = input('input: ').split(',')
print(var1, var2)
```
```
input: Hello, World!    # Hello, World! 입력
Hello  World!
```

> __NOTE__  
> `print()`에서 'Hello' 와 'World!' 사이에 공백 2칸이 있다.  
> 이를 통해 `var2`에 공백을 포함한 ' World!'가 저장된 것을 확인할 수 있다.
