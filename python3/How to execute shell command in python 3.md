# How to execute shell command in python 3


> environment : IDLE 3.8, Windows 10

<br>

__NOTE__
> 시작하기에 앞서, `IDLE editor`에서 작성된 코드를 바로 실행시키면 실행되지 않는다.  
> `cmd`를 이용해 작성된 코드를 실행해야 한다.

***

## os

```python
import os
```
`os` 모듈을 `import` 하면 `cmd` 에서 사용할 수 있는 명령어들을 사용할 수 있다.

```python
os.system(command)
```

`command`로 기술된 명령어를 실행한다.  
`dir` 이나 `python --version` 등 다양한 명령어를 실행하며 정상적으로 종료되면 0을 반환한다.

```python
import os
os.system('python --version')
```
```
Python 3.8.2
```

<br>

```python
import os
msg = 'echo hello'
os.system(msg)
```
```
hello
```

***
<br>

## subprocess

```python
import subprocess
```

`subprocess` 모듈은 몇가지 이전의 모듈들을 대체하기 위해 만들어졌다.  

<br>

```python
subprocess.run(args)
```

`args` 로 기술된 명령을 실행한다.  
`args` 는 리스트나 문자열일 수 있다.  
`args` 외에 더 많은 인자들이 있다.

 > `run()`함수는 파이썬 3.5 에서 추가되었다. 따라서 그 이전 버전은 `call()` 함수를 사용해야 한다.
 
 <br>
 
 ```python
import subprocess
args = 'python --version'
subprocess.run(args)
```
```
Python 3.8.2
```

<br>

```python
import subprocess
subprocess.run(['echo', 'hello', 'world'], shell=True)
```
```
hello world
```

`hello world` 를 출력하는 예제에서는 셸이 필요하므로 `shell=True` 를 추가해줘야 에러가 발생하지 않는다.  
또한 대부분의 명령어는 `shell=True` 를 추가해줘야 하는데, 그렇지 않을 경우 실행할 프로그램 이름으로 받아들이기 때문에  
다음과 같은 에러를 출력한다.

```python
import subprocess
subprocess.run(['echo', 'hello', 'world'])
```
```
Traceback (most recent call last):
~
~
~
FileNotFoundError: [WinError 2] 지정된 파일을 찾을 수 없습니다
```

***

__Reference__  
- [python Docs](https://python.flowdas.com/library/subprocess.html)
