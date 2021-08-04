# MySQL
mysql 정리

실행환경 mysql  Ver 8.0.26 for macos11.4 on arm64 (Homebrew)
mysql workbench Ver 8.0.25

작성환경 vscode python 3.8.6 | packaged by conda-forge | (default, Jan 25 2021, 22:55:00) [Clang 11.0.1 ]
(vscode 에서 python version 확인하기) 
```
import sys
print(sys.version)
```
(mysql version 확인방법)
mac terminal 에서 mysql --version

(mysql workbench version 확인방법)

workbench -> preferences ->modeling->mysql->default target mysql version 에서 확인


설치방법:
1.홈페이지에서 다운로드  
2.homebrew로 설치(권장) -이유는 m1 mac 환경에서 설치도중 다운되는 현상이 가끔발생함 개발의 시작은 설치+환경세팅인데 여기서막히면 stress받음   


brew search mysql -> 설치가능한 mysql 버젼이나옴   
brew install mysql@x.x -> 설치하고싶은 mysql 버젼 다운로드(x.x에 원하는버젼넣기)  
brew list -> 설치후 homebrew로 설치된 list 를 볼수있음   
-----설치완료후---------  
mysql.server start -> 서버스타팅  

mysql_secure_installation -> password 강도 선택후 비밀번호 -- 설정 끝  
mysql -uroot -p  -> 로그인하기  

finished!! 

하지만 terminal 에서의 작업은 너무 힘들기때문에
mysql workbench 다운로드를 강력하게 권장함
https://dev.mysql.com/downloads/workbench/ 에서 다운받으면됨.


