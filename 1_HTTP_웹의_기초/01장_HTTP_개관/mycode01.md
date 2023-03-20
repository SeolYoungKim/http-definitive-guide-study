### Q1. 파라미터와 쿼리스트링의 차이 
책에서는 다음과 같은 URL을 이렇게 설명할수 있다고 한다.

```
https://www.example.com/book/;sale=false/necronomicon;chapter=2
```
https scheme 을 이용해   
www.example.com 의 80 포트로 접근  
/book/necronomicon 리소스에 를 가져오되,  
book 의 메타데이터 sale 은 false 이고  
necronomicon 의 메타데이터 chapter 는 2 이다.


그런데, 웹 개발자로서 일반적으로 접했던 서버에 파라미터 전송은 다음과 같았다.
```
https://www.example.com/book/necronomicon?sales=false&chapter=2
``` 
물론 책에서 chapter 2를 쿼리해올수 있느냐는 구현에 따라 다르긴 하겠지만 암튼 이런 방식을 많이 사용했을 것이다.

그렇다면 파라미터(;사용)와 쿼리스트링(?과 &의 조합)은 무슨 유의미한 차이가 있는가?

잠깐 검색해 본 바로는 서버로의 질의, 그리고 리소스 접근데 대한 메타데이터(힌트?) 제공 이라고 하는데 잘 모르겠음.
