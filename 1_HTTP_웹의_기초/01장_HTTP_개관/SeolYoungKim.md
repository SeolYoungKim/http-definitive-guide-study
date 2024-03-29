# 질문 
## telnet
- 회사에서 telnet으로 ip 주소 및 포트에 접근이 가능한지 확인을 하는 작업을 했습니다. 하지만, 찾아보니 telnet은 거의 사용되지 않으며, ssh를 주로 사용한다고 합니다. 
- 그런데, 회사에서 ip:port에 접근이 가능한지 확인하는 용도로 telnet 명령어를 사용한 것 처럼 또 다른 이용처가 있을수도 있다고 생각합니다. 혹시 현업에서는 어떠한 용도로 사용되는지가 궁금합니다. 

## 1장 21p 1.8.4 터널
- 터널이란, 두 커넥션 사이에서 raw 데이터를 열어보지 않고 그대로 전달해주는 HTTP 애플리케이션임.
  - 주로, 비 HTTP 데이터를 하나 이상의 HTTP 연결을 통해 그대로 전송 해주기 위해 사용.
- 웹 트래픽만 허용하는 사내 방화벽이 있음 
  - 방화벽은 웹 트래픽만 허용하기 때문에, 암호화된 SSL 트래픽은 HTTP 채널을 통해야만 목적지 서버로 전송할 수 있음 
  - 다음과 같은 순서로 전송
    1. 클라이언트가 HTTP를 통해 암호화된 SSL을 터널에 전송
    2. 터널 시작
    3. 암호화된 SSL이 HTTP 커넥션을 통해 전송 됨
    4. 터널 끝 
    5. 암호화된 SSL이 SSL 커넥션을 통해 서버로 전송 됨

- "터널"이라는 것이 "무언가를 우회"하기 위한 방법으로 사용이 되는것인가요?
  - 위 예시의 경우, 웹 트래픽만 허용하는 방화벽을 넘어 암호화된 SSL을 서버로 전송하는 것이 목적이였기 때문에, HTTP 터널을 통해 SSL을 전송합니다.
  - 이는 웹 트래픽만 허용하는 방화벽을 "우회"한다고 이해했습니다.
- "우회"한다는 표현이 정확한 표현이 아닐 경우, 어떤 방법이라고 이해하면 될까요? (아래와 같은 표현이 떠올랐지만, 터널에 대한 정확한 이해가 좀 어렵네요.. ㅠ 너무 추상적인듯 합니다.) 
  - 그냥 터널의 역할이다. 웹 트래픽만 허용하는 방화벽을 지나기 위한 터널일 뿐. 
    - 그렇다면, 터널이 방화벽에 있는걸까요? 

