# README-File-Assingment
How to use Linux commands and vim editor macros

# 리눅스 명령어
---
# ***top (table of processes)***

* CPU 와 메모리 이용에 관한 정보를 표시하는 수많은 유닉스 계열 운영 체제에서 볼 수 있는 작업 관리자 
	프로그램
	
|옵션|내용|
|-----|-----|	
|shift + p | CPU 사용률 내림차순|
| shit + m | 메모리 사용률 내림차순|
| shift + t | 프로세스가 돌아가고 있는 시간 순|
| k | kill. k 입력 후 PID 번호 작성. signal은 9|
| f | sort field 선택 화면 -> q 누르면 RES순으로 정렬|
| a | 메모리 사용량에 따라 정렬|
| b | Batch 모드로 작동|
| 1 | CPU Core별로 사용량 보여줌|

### [top자료 출처](https://zzsza.github.io/development/2018/07/18/linux-top/ "top Explanation")
---

# ***PS(Process Status)***
* 현재 실행중인 프로세스 목록과 상태를 보여줌

|옵션|내용|
|-----|-----|
|-e|실행중인 모든 프로세스의 정보를 출력한다.|
|-f|프로세스에 대한 자세한 정보를 출력한다.(PPID 확인 가능)|
|-u [사용자이름]|특정 사용자에 대한 모든 프로세스의 정보를 출력|
|-p pid|pid로 지정한 프로세스의 정보를 출력|
|u|프로세스 소유자의 이름,CPU 사용량,메모리 사용량 등 상세 정보를 출력|
|a|터미널에서 실행한 프로세스의 정보를 출력|
|x|실행 중인 모든 프로세스의 정보를 출력|
### [PS자료 출처](https://blog.naver.com/PostView.nhn?isHttpsRedirect=true&blogId=jsky10503&logNo=220728880785&parentCategoryNo=&categoryNo=109&viewDate=&isShowPopularPosts=false&from=postView "PS Explanation")

---
# ***jobs***
* 작업이 중지된 상태, 백그라운드로 진행 중인 작업 	상태, 변경 되었지만 보고되지 않은 상태 등을 표시하는 	명령어

|옵션|내용|
|-----|-----|
|-l|프로세스 그룹 ID를 state 필드 앞에 출력|
|-n|프로세스 그룹 중에 대표 프로세스 ID를 출력|
|-p|각 프로세스 ID에 대해 한 행씩 출력|
|command|지정한 명령어를 실행|

### [jobs자료 출처](https://hbase.tistory.com/265 "jobs Explanation")

---
# ***kill***
* 프로세스에 특정한 signal을 보내는 명령어
### 주요 시그널

|시그널|영어|설명|
|-----|-----|-----|
|1) SIGHUP|Hang Up|세션이 종료될 때 시스템이 내리는 시그널|
|2) SIGINT|Interrupt|Ctrl + C,종료 요청 시그널|
|9) SIGKILL|Kill|강제 종료 |
|11)SIGSEGV|Segment Violation|메모리 침범이 일어날 때 시스템이 보내는 시그널|
|15)SIGTERM|Terminate|기본 값,종료 요청 시그널|
|20)SIGTSTP|Temporary Stop|Ctrl + Z,일시 중지 요청 시그널|

|옵션|내용|
|-----|-----|
|-l|signal의 종류를 출력한다.|
### 사용예
* kill [옵션 or 시그널(번호 or 이름)] PID
* kill -9 1234
* kill -SIGKILL 1234
* kill 명령어 뒤에 시그널 이름이나 숫자를 제외하고 실행하면 TERM(15번) signal 이 전송된다

### [kill자료 출처](https://jhnyang.tistory.com/143 "kill Explanation")
---

# vim 에디터에서 매크로 사용방법

![macro](https://user-images.githubusercontent.com/106680760/171987897-1af9f981-9ca5-4903-b8d8-e34dee316047.PNG)

### [macro자료 출처](https://clem.tistory.com/29 "macro Explanation")
