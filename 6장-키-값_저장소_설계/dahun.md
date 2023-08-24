# 6장 키-값 저장소 설계

- 해시 키 대신 일반 텍스트 키를 사용하는 것
  - [같은 텍스트 일 경우 hashcode가 똑같다](https://jithub.tistory.com/302)

<br>

- 정답은 분산처리, AP, 해시 링인가?
  - 4장 의문과 같은 맥락

<br>

- 일시적 장애 처리 이해 과정
    - 메시지 큐 같이 요청을 남겨두어서 서버가 살아났을때 재배치?

<br>

- 트리의 컨셉에 대한 새로운 시야
  - 해시 테이블을 사용하지 않는 이유 [1](https://jiwondev.tistory.com/112), [2](https://foot-develop.tistory.com/56)
  - 노드를 나눠 찾기 쉽게 만들기
  - [머클트리](https://www.lesstif.com/security/merkle-tree-125305097.html)
  - 데이터 조회의 끝판왕은 트리구조인가

<br>

- 데이터 버저닝
  - 구글 클라우드, 노션