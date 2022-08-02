# 💻  Linux Command5
## ✨Vi Editor
#### 1. Command Mode
 `vi명령어로 vi를 시작
 방향키를 이용하여 커서를 이동
 dd, yy, x 등 삭제 관련 명령어 사용 가능`
 ```
📍 Command
  i : 현재 커서 위치에 삽입(Insert Mode로 넘어감)
  a : 현재 커서 바로 다음위치에 삽입(Insert Mode로 넘어감)
  o : 현재 줄 다음 위치에 삽입(Insert Mode로 넘어감)
  x : 커서가 위치한 곳의 글자 1개 삭제 (3x : 문자 3개 삭제)
  dw : 커서가 위치한 곳부터 단어 삭제 (커서가 위치한 곳부터 띄어쓰기까지)
  dd : 커서가 위치한 곳의 한 줄 삭제 (p로 복구 가능)
  u : 방금 입력한 명령 취소
  yy : 현재 줄을 버퍼로 복사 (5yy : 5줄 복사)
  p : 현재 커서가 있는 줄 바로 아래에 버퍼 내용 붙여넣기
  k : 커서가 한 줄 위로 이동
  j : 커서가 한 줄 아래로 이동
  l : 커서가 한 칸 우측으로 이동
  h : 커서가 한 칸 좌측으로 이동ㅊ
  0 : 커서가 있는 줄의 맨 앞으로 이동
  $ : 커서가 있는 줄의 맨 뒤로 이동
  ( : 현재 문장의 처음
  ) : 현재 문장의 끝
  { : 현재 문단의 처음
  } : 현재 문단의 끝
  숫자- : 숫자 만큼 윗 줄로 이동
  숫자+ : 숫자 만큼 아래 줄로 이동
  G : 파일의 끝으로 이동 (대문자)
  r : 한 문자 변경
  cc : 커서가 있는 그 줄의 내용 변경
 ```

#### 2. Insert Mode
 `Command Mode에서 i 또는 a 통해 입력모드로 변경 가능
 자유롭게 코드 작성 가능
 Command Mode로 돌아올땐 ESC`

#### 3. Last Line Mode
 `Command Mode에서 ':' 입력시 저장 또는 종료 등을 입력 가능`
 ```
📍 Command
  w : 현재 파일명으로 파일 저장 (종료X)
  w 파일명 : 입력한 파일명으로 파일 저장 (종료X)
  q : vi 종료 (저장X)
  q! : vi 강제 종료 (!붙으면 강제)
  wq : 저장 후 종료
  wq! : 강제 저장 후 종료
  f 파일명 : 파일이름을 '파일명'으로 변경
  숫자 : 해당 라인으로 커서 이동
  $ : 파일의 맨 끝 줄로 이동
  e! : 마지막 저장 이후 모든 편집 취소
  /문자열 : 현재 커서 위치에서부터 파일 앞쪽으로 문자열 탐색
  ?문자열 : 현재 커서 위치에서부터 파일 뒤쪽으로 문자열 탐색
 ```