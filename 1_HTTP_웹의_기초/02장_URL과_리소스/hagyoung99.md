### 32p) 사용자 이름과 비밀번호

많은 서버가 자신이 갖고 있는 데이터에 접근을 허용하기 전에 사용자 이름과 비밀번호를 요구한다.
FTP 서버가 좋은 예다. 여기 몇가지 예가 있다.

- ftp://anonymous:my_passwd@ftp.prep.ai.mit.edu/pub/gnu
- http://joe:joespasswd@www.joes-hardware.com/sales_info.txt

예시는 아래의 두가지만 작성하였는데 본문에는 세 번째 예에 대한 내용은 나와있지만 HTTP URL에 대한 설명이 없습니다.
그동안 URL을 봐오면서 사용자 아이디와 비밀번호를 붙이는 경우를 보지 못했는데 어떤식으로 동작하는지 궁금합니다.


### 38p) 기저 URL과 절대 URL

37페이지의 그림 2-4에서는
http://www.joes-hardware.com/tools.html 이 기저 URL이 되고, 
./hammers.html 이 상대 URL이 되어 최종적으로는 http://www.joes-hardware.com/hammers.html 이 새로운 절대 URL이 된다고 나와있습니다.

그리고 38페이지에서는
기저 URL이 없는 경우도 있다. 보통 이런 경우는 절대 URL 만으로 이루어져 있다는 뜻이다. 하지만 불완전하거나 깨진 URL일 수도 있다.
고 나와있는데 그럼 기저 URL이 어떤거고 기저 URL이 없는 경우 절대 URL은 어떤 값이되는건지 이해하지 못했습니다.
