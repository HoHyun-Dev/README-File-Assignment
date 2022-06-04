# README-File-Assingment
How to use Linux commands and vim editor macros

# 리눅스 명령어
---
## top (table of processes)

* CPU 와 메모리 이용에 관한 정보를 표시하는 수많은 유닉스 계열 운영 체제에서 볼 수 있는 작업 관리자 
	프로그램
* shift + p : CPU 사용률 내림차순
* shit + m : 메모리 사용률 내림차순
* shift + t : 프로세스가 돌아가고 있는 시간 순
* k : kill. k 입력 후 PID 번호 작성. signal은 9
* f : sort field 선택 화면 -> q 누르면 RES순으로 정렬
* a : 메모리 사용량에 따라 정렬
* b : Batch 모드로 작동
* 1 : CPU Core별로 사용량 보여줌

### [top자료 출처](https://zzsza.github.io/development/2018/07/18/linux-top/ "top Explanation")
---

# PS(Process Status)

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
