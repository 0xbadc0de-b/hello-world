비박스(bee-box) bWAPP 워게임

# 1. 다운로드 및 설치

다운로드는 아래 검색어 및 URL 통해서 받으면 됨 
bWAPP - Browse /bee-box at SourceForge.net
https://sourceforge.net/projects/bwapp/files/bee-box/

설치는 가상이미지 다운 받으면 끝
http://stupidsecurity.tistory.com/23

설치후 체크사항
- 가상 머신의 네트워크는 NAT로 설정해야 함
- 키보드는 초기에 벨기에어로 설정되어있으므로, Preference->Keyboard->Layouts->Add-> Korea Republic of로 설정
- 접속 패스워드 : bee / bug
- 소스코드 위치 : /var/www/bWAPP


	
# 2. [low] HTML Injection - Reflected (GET)

Payload
```
<h1><a href="http://www.google.com">click me</a></h1>
<h1><img src=# onmouseover=alert(1004)></h1>
<img src="http://192.168.30.140/bWAPP/images/bee_1.png">
```

