[![42 Seoul](https://img.shields.io/badge/42seoul-000000?style=for-the-badge&logo=42&logoColor=white)](https://profile.intra.42.fr/users/jijeong)

# About Me

블랙박스 밖에서의 구현에 만족하지 못하고 실제 컴퓨터에서 프로그램이 어떻게 동작하고 관리되는지 이해하기 위해 학습해나가는 개발자입니다.<br>

[42서울(42seoul)](#ecole42)의 6기 수료생입니다. 프로젝트를 분석해 요구 조건을 명확히하고 각 상황에서의 예외처리를 정리해 구현하고 프로그램의 구조에 따라 시점에 따른 데이터를 고려하며 개발합니다. 또한 본과정 기준 121회의 동료평가의 경험([활동 기록](./42log.md))을 통해 타인의 코드를 이해하거나 본인의 코드를 설명하는 것에 능숙합니다.<br>



## Experienced
> 요구사항 분석, 설계, 예외처리, 구현의 모든 과정을 직접 진행하여 프로젝트를 완성한 경험
### Language & Project
#### C (c99) 
> 42의 C coding convention인 `Norm` 준수, `leaks`를 통한 메모리 누수 검증
- [miniRT](https://github.com/kiryud/miniRT) (2인/33일)
	- 3D 레이트레이싱(Phong Lighting) 구현 프로젝트
	- light, sphere, cylinder 구현
- [minishell](https://github.com/kiryud/minishell) (2인/36일)
	- 나만의 shell을 만드는 프로젝트
	- builtin command를 제외한 나머지 실행 영역 구현
		- tokenizer(parsing)
		- pipe, redirection 처리 및 fd 관리
		- 프로세스 분기
		- PATH 기반 명령어 존재, 실행가능성 탐색 및 실행(execve)
- microshell (Exam-Rank-04)
	- 제한시간 : 3시간
	- tokenized args를 기반으로 `|` `;`을 해석하여 실행시키는 시험
	- fd의 최대치가 제한된 환경에서의 fd lifecycle 심화 학습
 	- redirection이 따로 없고 pipe만 적용하면 되기 때문에 `;`를 기준으로 반복을 돌리고 `|`를 기준으로 fd를 설정하는 반복문이 동작함
  	- args가 사실상 cmds `|` or `;` cmds 구조이기때문에 각 루프마다 cmds의 0번째 index를 파악하여 기호가 있는 영역에 '\0'을 삽입 후 execve에 넣어 실행 과정 중 문자열을 위한 memory allocation을 피함
  	- fd의 최대 개수를 10개 미만으로 제악하는 테스트케이스가 있어서 고민하다 명령줄의 모든 pipe를 한번에 여는것이 아니라 임의의 명령어를 실행할 땐 앞에 있는 pipe와 뒤에있는 pipe의 두 쌍의 pipe가 있으면 된다는것을 알게됨
- mini_serv (Exam-Rank-06)
	- 제한시간 : 3시간
	- `select`를 기반으로 구현
	- 연결 순서대로 ID를 부여받는 echo chatting server 제작
   	- 10만 단위의 data를 전송해야했어서 buffer를 굉장히 크게 만들어봄
#### C++ (c++98)
> `OCCF`(Orthodox Canonical Class Form) 준수
- [ft_irc](https://github.com/kiryud/42_ft_irc) (3인/55일)
	- 상용 클라이언트 프로그램과 소통 가능한 단일 irc서버 제작
	- IRC 프로토콜 분석 및 Irc 로직 구현
		- RFC 1459, RFC 2812 기반 명령어 동작 및 RPL MSG 정리
		- RFC 문서에 생략된 실제 client의 해석 방식을 알아보기 위해 상용 서버와 irssi의 통신 분석
		- nc를 통한 client에서 동작의 트리거가 되는 메세지가 뭔지 분석
	- Server객체와 Irc객체 분리 및 호출 case 정의
#### JavaScript (SPA / WebSocket / Three.js)
- ft_transcendence ([tini-pong](https://github.com/kiryud/tini-pong)) (5인/61일)
	- pong 게임 구현
	- SPA 구조 기반 클라이언트 개발
	- WebSocket을 통한 온라인 멀티 플레이 구현
	- Three.js 활용

#### Architecture
- [Inception](https://github.com/kiryud/inception) (55일)
	- Docker Compose (env / network / volume)
	- LEMP (Alpine / Nginx / MariaDB / WordPress)
	- Nginx / MariaDB / WordPress 컨테이너를 Alpine 컨테이너 기반으로 Dockerfile 직접 구현

## Community
### with 42seoul
- [팔만코딩경](https://80000coding.oopy.io/f986d574-dea8-4197-bb7f-ee94af020a44)
- 수요지식회(발표)
    - [termux](https://github.com/kiryud/termux_setting) 갤럭시 탭을 활용해서 c 과제를 하고있었는데 관심가져주시는 분들이 많아서 간단하게 왜 가능하고, 어떻게 할 수 있는지 발표했다. 발표자료는 잃어버렸지만 그때 쓴 레포는 남아있다.
	- ford-johnson algorithm ([cpp-module-09 ex02](./fja.md)) 이것도 마찬가지로 알음알음 나한테 질문해주시는분들이 생겨서 발표했었다.
   		- [cpp-module-04~09](https://github.com/kiryud/cpp)해당 과제가 있는 레포

## Tool
- git / github
- vim / vsc
- linux (ubuntu / debian / alpine)
- shell script (bash / zsh)
- docker / docker-compose / colima / qemu
- slack / notion / obsidian

## Learning
> 예제 및 실습을 통해 학습한 경험
### Language & Project
- JavaScript (React)
	- [semicapstone](https://github.com/kiryud/semicapstone)
	- API를 활용한 간단한 대시보드 웹 페이지 제작
- Java (spring)
	- docker-compose로 mariaDB 이미지를 통해 init.sql로 데이터베이스, 테이블 구성
	- Entity / Dao / Service / Controller 구조 기반 DB 연동 CRUD JSP 웹사이트 구현
- python (django channels)
	- ft_transcendence에서 django channels를 기반 WebSocket 연결 이후의 메세지 처리 작성
- C# (ASP.net Core / Window Forms / LINQ / RabbitMQ)
	- 임의의 data를 json으로 변환하여 MQ에 보내는 Window Forms App
	- MQ로부터 메세지를 받아와 json을 해석해 화면에 출력해주는 Window Console App
- Kotlin (android / spring boot)
	- recyclerview 기반의 사진첩 앱 실습
	- intent를 기반으로 한 화면 이동시 데이터 전송
   	- spring boot는 학습중
- Dart (Flutter)
	- [unitask](https://github.com/kiryud/unitask)
		- 목업 디자인을 기반으로 MVVM 패턴 앱 제작 과정 학습
  		- 주차별 진행과 그 과정에서 배운것은 vault 디렉토리에 존재


# Contact
```
정진석 (Jeong JinSeok)
email : lundagran@gmail.com
```

## ecole42
ecole 42는 학비, 교재, 교수가 없는 3무 학습과 동료평가를 기반으로 PBL이 진행되는, 세계 혁신 대학(WURI) 3위의 대학교입니다.<br>
42서울은 그런 ecole42의 교육 커리큘럼을 들여온 이노베이션아카데미에서 제공하는 교육과정입니다.<br>
ecole42 및 42서울의 수료 조건인 공통과정(Inner Circle)은 C, C++를 기반으로 c string library부터 IPC, signal, data structure, algorithm, graphic, network를 거쳐 server programming까지 익힌 후 pong 게임 웹사이트를 만드는 것입니다.<br>
공통과정 통과 이후 42 network 소속으로 계속 남아 추가적인 학습을 지속할 수 있습니다.<br>
각 프로젝트는 최소 3명의 동료에게 평가받아야하며 평가시 코딩 컨벤션을 준수했는지, 메모리 누수가 없는지, 요구 조건에 맞게 동작하는지, 평가자에게 자신의 설계와 코드를 설명해 cheating 없이 본인의 능력으로 분석, 설계, 구현이 진행되었는지 검증받게됩니다.<br>
42서울의 교육과정을 통해 다른 사람의 코드를 이해하고 내 코드를 설명하며 평가 혹은 교류를 통해 알게 된 지식을 내 코드에 접목시키고 다들 놓치고 혼자 알아낸 지식을 퍼뜨리는 경험을 할 수 있었습니다.<br>

---

### Notes
#### [All Project List](./project.md) (작성중)
#### [All Skill List](./skills.md) (작성중)
