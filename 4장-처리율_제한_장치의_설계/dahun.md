# 4장. 처리율 제한 장치의 설계

### 각 장의 모범 답안은 분산 설계인가?
- 각 장마다 결국 대용량 처리를 위해서 분산 시스템을 구축하게 된다.
  - [Stackoverflow의 사례](https://blog.insane.pe.kr/1587)
  - [Segment의 사례](https://www.ciokorea.com/news/39258)

> 결국 MSA의 한계를 꼽는 것이 아닌 구현의 난이도나 비용문제 등을 짚는 걸 보니 완벽한 구축이 된다면 MSA만한게 아직 없는 것 같다.

<br>

- 계산 알고리즘의 필요성
  - 논리적 알고리즘 뿐만 아니라 단순 계산을 요구하는 알고리즘도 필요한 것 같다.
  - [Quake 3 알고리즘](https://ko.wikipedia.org/wiki/%EA%B3%A0%EC%86%8D_%EC%97%AD_%EC%A0%9C%EA%B3%B1%EA%B7%BC)
<br> 


- iptables
  - [iso 3레이어 수준의 처리율 제한](https://remybaek.tistory.com/117)
- nginx 에서의 트래픽 제한
  - [osi 7레이어 수준의 처리율 제한](https://ko.linux-console.net/?p=2673#gsc.tab=0)

<br>

- 동시성 이슈
  - [자바 응용](https://velog.io/@msung99/Redis-%EB%B6%84%EC%82%B0-%EB%9D%BD%EC%9D%84-%EA%B5%AC%ED%98%84%ED%95%B4-race-condition-%EB%8F%99%EC%8B%9C%EC%84%B1-%EC%9D%B4%EC%8A%88-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0)
  - [lua](https://hyperconnect.github.io/2019/11/15/redis-distributed-lock-1.html)

<br>

- 중앙 집중형 데이터 저장소도 분산 환경이 된다면 어떻게 될까
  - 요청 서버를 여러대 설정해서 분산 요청 가능하다.