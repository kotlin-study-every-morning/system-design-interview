### 다중마스터 복제
  - 다중마스터 복제 auto increment 방법
  - 서버1: 1부터 서버 갯수씩 증가, 서버2: 2부터 서버 갯수씩 증가
### uuid
  - 왜 갑자기 64비트 제한? 트위터를 위한 끼워맞추기?
    - 저자의 시간 관계상, 다양한 방법 설명을 위함
  - ULID라는 방법도 있다.
    - UUID + 순서
### 티켓 서버

### 트위터 스노 플레이크
  - 일련번호가 왜 필요할까?
    - 타임스탬프로도 감당할 수 없는 요청이 들어올 경우를 대비한다.
### ntp서버 + 나노시간
  - ntp서버를 통한 nano시간 동기화
  - https://www.rfc-editor.org/rfc/rfc958
    - 1항목 나노시간 동기화를 위함 기술되어있음
  - https://fsmlabs.com/140-nanosecond-worst-case-ntp-performance-with-timekeeper/
    - 최악 시간차는 140나노초
  - pk를 나노시간으로 처리 한다면 어떨까?