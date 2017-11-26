# Google Sign-in 설정하기

1. https://developers.google.com/identity/sign-in/android/start-integrating 에 들어간다

2. 아래의 버튼을 클릭한다.

![](/res/1.png)

3. App 이름과 패키지명을 입력한다.

![](/res/2.png)

4. How do I find my SHA-1?을 클릭한다.

![](/res/3.png)

5. mac이면 mac용 window는 window용으로 cmd에 입력한다. 그러면 아래와 같은 코드가 발행된다.

![](/res/4.png)

6. 칸안에 입력하고 버튼을 클릭한다. - 그리고 활성화 되는 버튼을 클릭한다.

![](/res/5.png)

7. 이제 google-services.json을 다운받고 project의 app 폴더에 넣는다.

![](/res/8.png)

8. 아래의 그림대로 gradle설정을 해준다.

![](/res/9.png)

9. 다음으로는 OAuth의 web Client를 생성하기 위해 Credentials page에 들어간다.

![](/res/10.png)

10. 사용자 인증정보 만들기 -> OAuth 클라이언트 ID 클릭

![](/res/12.png)

11. 웹 어플리케이션 선택 후 이름을 맘대로 지어주시고 생성

![](/res/13.png)

12. 마지막으로 발급받은 클라이언트 아이디만 Strings 안에 아래와 같이 넣는다
````
<string name="server_client_id">your key</string>
````

이것으로 설정은 완료