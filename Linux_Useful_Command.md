# 💻 Useful Command

📍Unix에는 Bourne Shell, Bash, fish, zsh 등 많은 shell등이 존재
하나만 잘 사용해도 shape들이 비슷해서 나머지도 사용 가능

### ✨ Manual and Navigating file system
```
$ man : manual 확인
$ clear : terminal의 모든 명령어들을 지움
$ pwd : Print Working Directory 약자, 현재 경로 알려줌
$ ls : 현재 경로의 폴더/파일 보여줌
$ ls -l : long, 폴더/파일의 자세한 정보
$ ls -a : all, 숨겨진 파일/폴더까지 표시
$ ls -la : 숨겨진 파일/폴더의 디테일
$ open . : 현재 경로를 파일탐색기에서 오픈
$ cd 파일명: Change Directory, 현재 경로 위치를 변경
$ cd .. : 현재 경로의 상위 경로로 변경
$ cd ~ : 최상위 경로로 이동
$ cd - : 이전 경로로 이동
$ find 파일명 : 특정한 파일/디렉터리를 찾을때
$ find . -type file -name "*.txt" : type이 file이고 이름이 txt확장자로 끝나는 file 탐색
$ which : 실행하고자 하는 파일이 어디에 설치/실행 경로 확인
```

### ✨ Create and manage file
```
$ touch 파일명 : 파일 생성
$ cat 파일명 : 파일 내용 확인
$ echo "문자열" : 문자열을 터미널에 다시 출력
$ echo "문자열" > 파일명 : 문자열을 파일에 덮어씀
$ echo "문자열" >> 파일명 : 문자열을 파일에 덧붙임
$ mkdir 이름 : Directory 생성
$ mkdir -p 경로 : 작성된 경로에 없는 directory는 자동 생성

$ cp 파일명 경로 : 파일을 경로로 복사
$ mv 파일명 경로 : move, 파일을 경로로 이동
$ rm 파일명 : remove, 파일 삭제
$ rm -r 디렉터리명 : directory 삭제

$ grep "키워드명" *.txt : Global Regular Expression Print, 지정한 키워드 검색해 출력
$ grep -n "키워드명" *.txt : 행 번호까지 출력
$ grep -ni "키워드명" *.txt : 대소문자 관계없이 행 번호와 출력
$ grep -nir "키워드명" . : 모든 경로에서 키워드 검색해 대소문자 관계없이 행 번호와 출력
```

### ✨ Work with environment variables
`환경 변수 : 내 컴퓨터에서 특정한 키워드가 어떤한 일을 하거나 경로를 저장할 수 있도록 만듦`
```
$ export MY_DIR="디렉터리명" : MY_DIR는 지정한 디렉터리라는 것을 설정
$ env : 설정된 모든 환경변수 출력
$ cd $MY_DIR : MY_DIR로 지정한 디렉터리로 이동
$ unset MY_DIR : MY_DIR로 지정한 환경변수 해제
```