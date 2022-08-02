# 💻  Linux Command3
```
$ sudo su - : super유저로 변경(root, 비밀번호 입력 요구됨)
$ exit : super유저 로그 아웃
$ sudo passwd : 비밀번호 변경/설정
$ useradd 이름 : '이름'의 유저 생성
$ userdel -r 이름 : '이름'의 유저와 정보 삭제
$ passwd 이름 : '이름'의 유저의 비밀번호 변경/설정
$ su - 이름 : '이름'의 유저로 로그인

$ groupadd 이름 : '이름'의 그룹명 생성
$ tail /etc/group : 변경 사항 확인 가능
$ groupmod -n 이름1 이름2 : '이름2'그룹의 이름을 '이름1'로 변경
$ groupdel 이름 : '이름'그룹 삭제
$ gpasswd 이름 : '이름'그룹 비밀번호 변경/설정
$ gpasswd -r 이름 : '이름'그룹 비밀번호 삭제
$ gpasswd -a 유저명 그룹명 : 그룹에 유저 추가

$ chmod 숫자3자리 파일명 : '파일명'의 권한을 변경
 ex) chmod 000 test.java   //test.java를 아무 권한이 없는 파일로 변경
     (000:아래참조)
```

# 💻 사용권한 조회
`사용권한은 총 10자리`
__-rwxr-xr--__  
``` 
 ⇨ 첫번째 자리의 -또는 d는 파일인지 디렉토리(d)인지 나타냄
 ⇨ 나머지는 user, user group, everyone에 대해 read, write, execute 세가지 권한을 나타냄
  - / wxr   / r-x  / r--
   / 소유자 / 그룹  / 방문자
```
```
➔ Symbolic notation
r : 읽기(read)
w : 쓰기(write)
x : 실행(execute)

➔ Octal notation
 0 : No Permission
 1 : Execute
 2 : Write
 3 : Execute and Write (1+3)
 4 : Read
 5 : Read and Execute (2+3)
 6 : Write and Read (2+4)
 7 : Read, Write and Execute (1+2+4)
```