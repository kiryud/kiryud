# 0 Circle

```md
project : libft
Circle : 0
Language : C
Type : solo
introduce : C 문자열 라이브러리 제작
```

# 1 Circle

```md
project : get_next_line
Circle : 1
Language : C
Type : solo
introduce : 임의의 fd로부터 '\n'을 기준으로 한 줄을 반환하는 함수 제작
```

```md
project : ft_printf
Circle : 1
Language : C
Type : solo
introduce : 버퍼 없이 write를 기반으로 서식지정자를 해석해 작동하는 printf 제작
```

```md
project : Born2BeRoot
Circle : 1
Language : null
Type : solo
introduce : VM 위에 Linux를 설치 후 보안을 위한 기본 설정을 해보는 과제
```

# 2 Circle


```md
project : pipex
Circle : 2
Language : C
Type : solo
introduce : cli 환경에서 '|'를 사용하는 것이 내부적으로 어떻게 동작하는지 학습 및 구현
```

```md
project : so_long
Circle : 2
Language : C
library : mlx
Type : solo
introduce : 간단한 2d 게임 제작 및 맵 검증
```

> 맵 검증에 dps 사용 근데 n-queen 문제 풀어봤는데 이걸 못할리가 없지 않나?

```md
project : push_swap
Circle : 2
Language : C
Type : solo
introduce : 두개의 변형된 스택을 통한 정렬 최적화 알고리즘 제작 (push  swap  rotate  reverce_rotate)
```

> 임의의 수가 들어오는거라 순차적으로는 연결 리스트로, 동시에 트리에 넣어서 중위순회로 indexing 진행함

# 3 Circle


```md
project : minishell
Circle : 3
Language : C
Type : group(2)
introduce : 나만의 작은 shell 만들기
```

```md
project : philosophers
Circle : 3
Language : C
Type : solo
introduce : philosophers문제 해결을 위한 비동기 data race 방지 규칙 제작
```

# 4 Circle


```md
project : netPractice
Circle : 4
Language : Null
Type : solo
introduce : internet - 라우터 - 스위치 - 단말(터미널) 구조에서의 ip, 서브넷 마스크 할당 실습 과제
```


```md
project : miniRT
Circle : 4
Language : C
library : mlx
Type : group(2)
introduce : 점광원, 평면, 구, 원기둥을 기반으로 한 간단한 레이트레이싱 프로그램 제작
```

```md
project : cpp-module-00~04
Circle : 4
Language : CPP
Type : solo
introduce : OCCF 규격에 맞추어 간단한 객체지향 상속 과제를 통한 cpp 학습
```

# 5 Circle


```md
project : cpp-module-05~09
Circle : 4
Language : CPP
Type : solo
introduce : OCCF 규격에 맞춘 cpp STL 학습 과제
```

> 개인적으로 cpp-module과제 중 따로 빼서 내 스스로 잘 했다고 생각하는 문제
```md
project : cpp-module-09 ex02-PMergeME
Circle : 4
Language : CPP
Type : solo
introduce : STL에서 2가지 자료구조를 사용하여 특정 알고리즘을 실행시켜 그 시간을 비교해보는 과제
- 근데 이제 Ford-Johnson Algorythm (merge-insertion sort)를 구현해야하는
정보는 논문, 컴퓨터 공학 전공 서적 중 한 페이지, 위키피디아의 대략적인 설명 뿐
해당 알고리즘은 이진 탐색을 최소한도로 구현했던 시기가 있는 알고리즘임
설명으로는 야콥스탈 수열이 그 이진탐색을 최소 횟수로 유지하는 방식이라고 되어있음
개인적으로 그 설명에 납득할 수 없었음
탐색 횟수를 최소한도로 줄이려는 방식의 알고리즘을 연구하는데 수열을 사용하기 위해 접근했을리가 없다고 생각함
따라서 여러 테스트 케이스를 만들고 단계별로 어떤 동작을 하는 지 상세히 분석함 (뭔가 잡힐듯 말듯 해서 밤 새서 고민했었음)
이진 탐색을 최대한 적게 한다는 원리가 완전 이진 트리에서 depth가 같은 모든 형태에서 같은 탐색 횟수를 가지기때문에 같은 탐색 횟수를 유지할 수 있는 개수만큼 양보하여 역순으로 삽입하는 구조임을 밝혀냄
```

> 개인적으로 저게 중요한 경험인 이유가 백준 루비1에 삼성 코딩대회 우승해서 입사 확정나신 분이 내내 제대로 만든 사람이 없어서 다 fail주고 있어요라고 하면서 다니실 때 나 혼자 제대로 구현해내고 그 원리를 42네트워크에 뿌렸음. 그 시절에 연고대생도 꽤 있었는데도 놓치던 디테일이라는거 생각하면 아 내가 개발을 못 할 사람이 아니구나!라는 확신이 이 때 나왔었지

```md
project : inception
Circle : 5
Language : null
Type : solo
introduce : docker-compose를 활용하여 webServer(nginx), WAS(PHP - wordpress), DB(mariaDB)를 직접 alpine 기반으로 dockerfile을 작성하여 volume, network(bridge) 설정을 하는 과제
```

> 알파인 기반으로 특정 프로그램이 깔려있는 이미지가 굉장히 많은 것과 다르게 실질적으로 알파인에서 마리아 디비 관련 공식 문서가 너무 낡아서 호환이 안되는데 과제 규칙상 그런거 해결하라고 알파인 버전을 높여놔서 그걸 해결하기 위해 직접 docker에서 alpine을 띄워서 한줄한줄 설치과정을 정리하면서 dockerfile을 작성함 그리고 실행해서 터짐..... tty local 권한 문제때문에 그런 문제가 존재한다는 사실과 해결하는 방법을 같이 찾았어야 했었음

```md
project : ft_irc
Circle : 5
Language : cpp
Type : group(3)
start : 2024.01.12.(금)
finish (115) : 2024.02.13.(화)
finish (125) : 2024.02.21.(수)
introduce : irc protocol을 기반으로 작동하는 단일 서버 제작 (상용 클라이언트와 통신 가능)
```

```md
history : ft_irc

start : 2024.01.12.(금)

RFC문서 및 irc protocol 분석 : 2024.01.13 ~ 01.16
	- RFC문서에 RPL, ERR 메세지 규약이 제대로 없는 경우가 많음
		- 여러가지 RFC 문서 중 해당 부분을 발췌독
		- IRCprotocol의 RPL, ERR메세지를 기반으로 검색해 IRCv3같은것도 찾아냄
	- 확실한 검증을 위해 상용 irc서버와 irssi의 통신을 tcp 통신을 감?청해서 확인

1차 제작 : 2024.01.18 ~ 01.24

서버와 irc로직을 분리하기로 결정 : 2024.01.25
	- 서버 1명, irc 프로토콜 2명의 구성에서 서로의 개발 편의와 메모리 관리 등을 위하여 서버 객체와 irc 객체를 나누어 작성하기로 함
		- 서버에서 진행하는 kqueue의 구조를 배워 어떤 event처리가 가능한지 배움
		- 해당 event에서 진행해야하는 irc객체의 동작과 그 때 받는 정보와 반환할 정보를 정리함
		
서버와 irc로직을 분리하기 위한 각 객체의 책임과 역할 정리 : 2024.01.25 ~ 01.29

finish (115) : 2024.02.13.(화)
finish (125) : 2024.02.21.(수)

```

```md ft_irc
- RFC문서와 다양한 자료(특정 회사에서 만드는 irc 규약 버전)를 활용하여 IRC 표준 응답 코드를 명확하게 지킴
- 상용 서버와 상용 client(irssi)가 주고받는 메세지를 socket에서의 TCP 통신 내역을 log로 출력시킨 뒤 분석해 어떤 메세지가 의미를 가지고 어떤 메세지가 추가적인 정보에 해당하며 어떤 메세지를 해석해 ui를 꾸미는지 면밀하게 파악 후 구현함
- kquere를 사용했고 send/recv가 비동기적으로 일부분씩 주고받아지기때문에 개별적인 send buffer를 기반으로 받아두고 해석 가능한 최소 단위의 명령어 구성이 되었는지를 캐리지 리턴 기준으로 확인 후 파싱, 보내는 것도 buffer를 두어 안정성 확보.
```

# 6 Circle

```md
project : mini_serv (Exam-Rank-06)
Circle : 6
Language : C
Type : Exam
introduce :
```

```md
project : ft_transcendence
Circle : 6
Language : html/css/js python
Type : group(5)
introduce :
- 구성
	- frontend : vanilla JS
	- backend : Django (python)
	- DB : postgresSQL
- 요구 조건
	- 필수
		- SPA
		- Pong game
			- 1 vs 1
			- tournament
	- 선택
		- 3d pong game
		- multi user
```

```md
history : ft_transcendence

(팀 시작) : 2024.02.14
(팀 참가) : 2024.02.16 - 나는 이날 합류함 (프론트엔드)
(기초 학습) : ~ 2024.02.21 - 역할에 맞춰 각자 기본적인 언어, 라이브러리, 프레임워크 학습
(기획) : 2024.02.22 ~ 02.29
	- 내 역할 : pong game
(개발) : 2024.03.01 ~ 04.16
<!-- 1~3일 3일간 심한 감기에 걸려 앓아누웠음 -->
	- local pong game
		- start : 2024.03.04
		- threeJS 배우기
		- Key event 처리 : 2024.03.15
		- local pong game 제작 완료 : 2024.03.19
	-  remote pong game
		- pong game이 렌더링되는 위치 고민
		- websocket 학습 2024.03.24 ~ 2024.03.29
		- 제작 및 마무리
finish(125) : 2024.04.16
```

```md
outer project : python-piscine
Language : python
Type : solo
introduce : 간단한 파이썬 학습 과제
```

```md
outer project : quine
Language : C
Type : solo
introduce : 자기 자신의 소스코드를 출력하는 프로그램
```

