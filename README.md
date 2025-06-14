# 2024-Herethon-6
2024 여기톤 : HERETHON 6조


<h1>👨‍💻 Role & Contribution</h1>
<hr>

![image](https://github.com/user-attachments/assets/cb9ad053-37eb-4d37-b099-4b0e93ed90a8)


<hr>
Title
독창성 있는 티칭에 자신있거나 새로운 배움에 도전하고 싶은 MZ세대가 공존하는 1:1 맞춤 티쳐 매칭 웹 서비스
자신의 실력을 전수하고싶거나 나만의 티칭 능력을 발휘하고 싶은 MZ세대라면 이 서비스를 통해 멘토가 될 수 있습니다! 당신은 다양한 러너분들을 모시면서 창의적인 아이디어와 감각으로 나만의 티칭 능력과 경험을 쌓을 수 있어 의미있는 서비스가 될 것입니다.

가르침 받기를 원하시나요? 기발한 아이디어로 구상된 티칭을 배우고 싶은 MZ세대라면 러너를 추천드립니다. 러너분들이 원하는 티쳐의 타입과 관심있는 스킬 분야를 참고하여 1:1 맞춤 MZ 티쳐를 소개해드릴수 있습니다.

러너분들은 다양한 카테고리의 스킬 분야에서 MZ의 티칭을 접할 수 있고, 디지털 소통으로 이루어지는 티칭이므로 불필요한 관계 형성을 강요하지않기에 친목과 배움을 아우르는 완벽한 커뮤니티를 형성할 수 있습니다.

나만의 MZ 티쳐를 만나보고 싶다면 MZ의 스킬을 활용해보세요.
<hr>

![image](https://github.com/user-attachments/assets/f372bf6d-86dd-4e4e-bcde-a3bd8ff74ada)
![image](https://github.com/user-attachments/assets/bb5472ff-db8b-4957-9a70-c2e20c0a5e9b)
![image](https://github.com/user-attachments/assets/69410a63-19f3-4bd7-a9eb-3f837831bba5)
![image](https://github.com/user-attachments/assets/c4565fc4-69f8-4c4e-b0e3-d5175752032d)
![image](https://github.com/user-attachments/assets/9923fce5-bdb9-4a73-aea4-0f8e92ea264d)
![image](https://github.com/user-attachments/assets/83184a5a-fd6b-4bae-8463-b40312e6ac2d)
![image](https://github.com/user-attachments/assets/e8b2cbcf-de54-4437-99f0-5375207657ba)
![image](https://github.com/user-attachments/assets/34c9df14-633d-49c3-a023-042180412eac)
![image](https://github.com/user-attachments/assets/88c26b98-082c-4a75-b723-dce7d2462c98)
![image](https://github.com/user-attachments/assets/b394c373-ee18-4379-8b4d-fcfbbe0b64a7)
![image](https://github.com/user-attachments/assets/dc421d92-26d5-4c7a-87aa-cc2b1dbcca7e)
![image](https://github.com/user-attachments/assets/4d8f53ba-b4bf-4613-ba9c-232f5db6fb29)
![image](https://github.com/user-attachments/assets/79a68288-0ed0-4c9d-b42b-54d343ce3abf)
![image](https://github.com/user-attachments/assets/7d8e11b7-6c8b-44d7-a2ff-19379e3cf1f6)
<hr>
<li>폴더구조</li>

```
mzSkill/
├── accounts/
├── chat/
│   ├── __pycache__/
│   ├── migrations/
│   ├── templates/
│   │   └── chat/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── consumers.py
│   ├── models.py
│   ├── routing.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── community/
├── main/
├── matching/
├── media/
├── mzSkill/
├── profiles/
├── review/
├── static/
├── db.sqlite3
├── docker-compose.yml
├── Dockerfile
├── manage.py
├── requirements.txt
└── .gitignore
```


<li>개발환경 실행방법</li>

```
$ python -m venv myvenv    #가상환경 생성
$ source myvenv/Scripts/activate
$ pip install pillow
$ pip install django
$ cd mzSkill
$ docker-compose up
```
*Django에서 Channels라이브러리를 이용한 비동기 통신 과정을 진행했습니다.
요청-응답의 단방향통신과 구분되는 서버와 클라이언트간 메세지의 양방향 교환을 구현했으며 이를 통해 브라우저에서 WebSocket 서버로 요청이 들어오면 HTTP에서는 미리 구축해놓은 라우팅파일을 이용해 HTTP -> WS로 프로토콜을 전환 후 메세지 단위로 전달할 수 있습니다.*
