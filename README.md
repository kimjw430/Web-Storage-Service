# Web-Storage-Service 구동 방법

1. 소스를 다운받은 뒤 압축을 푼다.
2. 웹 페이지 소스를 gradle로 빌드한다.
(html 경로에서 명령 창을 연 뒤 gradle-2.13\bin\gradle build 명령으로 빌드할 수 있다.)
3. 빌드된 war파일을 apache-tomcat-9.0.0.M3_20160328\webapps 폴더로 옮긴다.
4. apache-tomcat에서 war 파일의 압축을 풀 때 java.lang.IllegalArgumentException 오류를 일으키므로 apache-tomcat을 켜기 전에 2번에서 옮긴 war 파일의 압축을 풀어준다.
5. mysql 서버를 구동한다.
(mysql-5.7.13-win32\bin\start-mysqld.bat 실행)
6. apache-tomcat을 구동한다.
(apache-tomcat-9.0.0.M3_20160328\bin\startup.bat 실행)
7. http://(톰켓 서버 주소):8080/wss로 접속한다.
