# 목차
1. [명세서와 매뉴얼](#명세서와-매뉴얼)
2. [Hello World!](#hello-world)
3. [Reference](#reference)
<br>

---
# 명세서와 매뉴얼
명세서와 매뉴얼은 기술을 공부하기 위해 필수로 봐야 한다.  
비록 영어로 되어 있어 보기 어렵고, 기초 수준의 내용은 검색만으로 간단히 해결이 가능하다.  
하지만 배우고자 하는 기술에 대해 더 깊고 자세하게 알기 위해선 검색만으로는 모자란 경우가 많다.  
그럴 경우를 대비하여 명세서와 매뉴얼을 이용해 원하는 정보를 찾는 연습을 해둬야 한다.  

- 명세서 [ECMA-262](https://tc39.es/ecma262/)
- 매뉴얼: [MDN.ko](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference)
- 매뉴얼: [MDN.en](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)
<br>

---
# Hello World!
`<script>`태그를 사용해 자바스크립트를 실행  
HTML문서 대부분의 위치에 삽입이 가능  

```javascript
<script>
  alert('Hello, world!');
</script>
```

자바스크립트 코드가 길어질 경우, 별개의 문서로 분리해서 저장  
`src`속성을 사용해 HTML에 삽입  
절대 경로, 상대 경로 둘다 가능  
```javascript
<script src="/path/to/script.js"></script>
```
```javascript
<script src="script.js"></script>
```

URL을 사용해 사입 가능  
여러개의 파일을 삽입하려면 `<script>` 태그를 추가하면 된다.
```javascript
<script src="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.11/lodash.js"></script>
```
```javascript
<script src="/js/script1.js"></script>
<script src="/js/script2.js"></script>
```

`src`속성을 사용하면 `<script>`태그 내부에 코드를 사용할 수 없다.
이를 해결하려면 두 개의 스크립트로 분리해야 한다.
```javascript
<script src="file.js">
  alert(1); // src 속성이 사용되었으므로 이 코드는 무시됩니다.
</script>
```

---
### 번외
- 여러개의 태그 예시문에서 태그 색상이 올바르게 출력되지 않는 이유 찾기

---
### Reference
[모던 JavaScript](https://ko.javascript.info/hello-world)
