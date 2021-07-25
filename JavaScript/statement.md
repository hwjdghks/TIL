# 목차
1. [statement](#statement)
2. [Reference](#reference)

---
# statement
statement(문): 실행 가능한 최소의 독립적인 코드  
`a = 3`  
`alert('Hello')`  

서로 다른 문은 세미콜론`;`으로 구분한다.  
`alert('Hello'); alert('World!');`  

줄바꿈이 있으면 '암시적' 세미콜론으로 해석  
이러한 방식을 `세미콜론 자동 삽입`이라고 부름
```html
alert('Hello')
alert('World!')
```  

하지만 모든 경우에서 작동하는 것은 아님  
따라서 각각의 문 끝에 세미콜론을 삽입하는 것을 권장
> 에러가 발생하는 구체적인 예시는 아래 레퍼런스 참고

---
# Reference
- [모던 JavaScript](https://ko.javascript.info/structure)
- [Expression과 Statement의 차이](https://shoark7.github.io/programming/knowledge/expression-vs-statement)
