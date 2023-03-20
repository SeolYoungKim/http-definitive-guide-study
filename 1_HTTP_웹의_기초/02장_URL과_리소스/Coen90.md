# 2.2.5 파라미터, 2.2.6 질의 문자열

## 질의문자열

URL에서 파라미터는 우리가 알고있던 Query String과 비슷하다.  
key/value 형태로 사용한다.  
질의 문자열은 http://www.http.com/test/test.html?key1=value1&key2=value2 와 같은 형식으로 URL의 마지막에 ?key=value 형태로 사용한다.   
일반적으로 가장 많이 사용하는 방식이다.  

  
## 파라미터

파라미터는 질의 문자열과 비슷하지만, 각 경로조각에 다 사용할 수 있다고 한다.  
http://www.http.com/test;key1=value1/test.html;key2=value2  



## 차이점
파라미터는 잘 사용하지 않는듯 한데, 위 둘의 차이점은 찾아봐도 시원한 답변을 볼 수 없었다.  
GET 요청의 경우 쿼리스트링으로 데이터를 전달하기에 상관이 없지만 POST 요청의 경우, 상황에 따라 누락이 되는 경우가 있을 수 있다고 합니다. [참고자료](https://stackoverflow.com/questions/39266970/what-is-the-difference-between-url-parameters-and-query-strings)  
그렇기에 HTTP Method나 Scheme에 따라 파라미터를 사용하는 경우가 있지 않을까 라는 궁금증이 생겼습니다. 다른 프로토콜은 사용해본적이 없기에 다른 프로토콜에서의 예시가 있는지 궁금합니다.


