# subprocess
## subprocess.run()


### error

```
AttributeError: 'str' object has no attribute 'fileno'
```

>stdin, stdout, stderr 에는 파일 이름이 아닌 파일 객체가 들어가야 한다.  
[stack overflow](https://stackoverflow.com/questions/31488688/attributeerror-str-object-has-no-attribute-fileno)  
