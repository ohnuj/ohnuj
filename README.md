<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,55:123D35,100:36D399&height=210&section=header&text=JUNHO.DEV&fontSize=58&fontColor=E6FFF5&fontAlignY=38&desc=BACKEND%20DEVELOPER%20%E2%80%A2%20JAVA%20%26%20SPRING&descSize=15&descAlignY=59&animation=fadeIn" alt="JUNHO.DEV — Backend Developer"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=19&duration=3000&pause=1300&color=36D399&center=true&vCenter=true&width=600&lines=Build.+Debug.+Improve.;Java+%26+Spring+%7C+Real-time+%7C+AI;Turning+ideas+into+working+services." alt="Build. Debug. Improve."/>

<br>

**아이디어를 구현하고, 동작을 확인하고, 끝까지 개선합니다.**

Java와 Spring을 중심으로  
실시간 통신과 AI 기능을 웹 서비스에 연결합니다.

<br>

<a href="https://github.com/ohnuj">
  <img src="https://img.shields.io/badge/GITHUB-0D1117?style=for-the-badge&logo=github&logoColor=36D399" alt="GitHub"/>
</a>
<a href="mailto:jjh980225@gmail.com">
  <img src="https://img.shields.io/badge/EMAIL-0D1117?style=for-the-badge&logo=gmail&logoColor=36D399" alt="Email"/>
</a>
<a href="https://github.com/ohnuj?tab=repositories">
  <img src="https://img.shields.io/badge/REPOSITORIES-0D1117?style=for-the-badge&logo=git&logoColor=36D399" alt="Repositories"/>
</a>

</div>

<br>

## `01` / NOW

<pre>
junho@dev:~$ cat focus.txt

BUILDING    실시간 채팅 · 인증 복구 · AI 서비스 연동
LEARNING    SQLD · FastAPI · LLM
NEXT        프로젝트 경험을 정리한 개인 포트폴리오
</pre>

<br>

## `02` / SELECTED WORK

### 🔒 SPOILOCK
#### 시청한 만큼 이야기하는 AI 스포일러 보호 커뮤니티

사용자별 시청 진도와 AI 판정을 연결해  
드라마 채팅·커뮤니티의 스포일러 노출을 제어하는 팀 프로젝트입니다.

| SERVICE | MY WORK |
| :--- | :--- |
| 실시간 토론방 · 자유방 · 비밀방 | 채팅 송수신, 참여자·초대·방장 위임·강퇴 |
| 드라마 시청 · 사용자 활동 | 영상 시청, 작품 상세, 마이페이지 |
| 커뮤니티 · 소셜 기능 | 신고·알림, 팔로우 연동, 사진 첨부 UI |
| 연결 및 운영 안정화 | 인증 복구, 반복 요청 제한, WebSocket 종료 처리 |
| 관리자 기능 | 저작권 이용 권한·증빙자료·변경 이력 관리 |

**Engineering Keywords**

`WebSocket / STOMP` `Redis Pub/Sub` `인증 상태 관리` `비동기 AI 연동`

<details>
<summary><b>프로젝트 기술 스택 보기</b></summary>

<br>

`Java` `Spring Boot` `Spring Security` `JPA` `QueryDSL`  
`React` `MySQL` `Redis` `FastAPI` `Gemini API`  
`AWS EC2` `Amazon S3` `GitHub Actions`

팀 전체 기술 스택이며, 개인 담당 범위는 위의 MY WORK에 구분했습니다.

</details>

<br>

**Repository · 포크 및 정리 예정　/　Demo · 업로드 예정**

<br>

---

### 🧠 Mood & Move
#### 감정 기록에서 시작하는 개인 맞춤형 행동 추천

<a href="https://youtu.be/KhvVEx4mxlc">
  <img src="https://img.youtube.com/vi/KhvVEx4mxlc/hqdefault.jpg" width="440" alt="Mood & Move 시연 영상 보기"/>
</a>

**감정·일기·취미·활동 선호를 바탕으로 Gemini가 행동 3가지를 제안합니다.**

| MY WORK | IMPLEMENTATION |
| :--- | :--- |
| 개인화 추천 | 유효 재측정 표본 수에 따라 Cold Start → Hybrid → Personalized 전환 |
| 추천 점수 설계 | 기분 변화량·긍정 변화 비율에 표본 수 기반 신뢰도 반영 |
| 응답 품질 관리 | 현재 상황 중심 프롬프트, 카테고리·시간·중복·장소 정보 검증 |
| 저장 일관성 | LLM 호출과 DB 저장 분리, 일기·추천을 하나의 MySQL 트랜잭션으로 저장 |
| 장소 검색·추적 | Kakao Local 연동, 캐시·재시도, MongoDB 요청·응답·실패 단계 기록 |

`Spring Boot` `React` `MySQL` `MongoDB` `Gemini API` `Kakao Local API`

**[Repository ↗](https://github.com/ohnuj/mood-and-move)　[Watch Demo ↗](https://youtu.be/KhvVEx4mxlc)**

<br>

---

### 🌱 지구비우기
#### 재활용 정보를 찾고, 실천하고, 보상받는 친환경 플랫폼

<a href="https://youtu.be/zqBimjOBDw8">
  <img src="https://img.youtube.com/vi/zqBimjOBDw8/hqdefault.jpg" width="440" alt="지구비우기 시연 영상 보기"/>
</a>

**재활용 정보·수거함 지도·커뮤니티 활동을 에코포인트와 리워드로 연결했습니다.**

| MY WORK | IMPLEMENTATION |
| :--- | :--- |
| 설계 | 화면 흐름·ERD·데이터베이스 구성 |
| 핵심 기능 | 재활용 정보 검색, 에코포인트 적립·사용·이력 관리 |
| 서비스 운영 기능 | 리워드 교환 및 관리자 처리 |
| 협업 | 팀장으로서 역할 분담과 진행 상황 조율 |

`Java` `Spring MVC` `MyBatis` `MySQL` `Thymeleaf`

**[Repository ↗](https://github.com/ohnuj/jigubium)　[Watch Demo ↗](https://youtu.be/zqBimjOBDw8)**

<br>

## `03` / TOOLBOX

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,react,js,mysql,redis,mongodb,docker,aws,git&perline=5" alt="Java, Spring, React, JavaScript, MySQL, Redis, MongoDB, Docker, AWS, Git"/>

</div>

<br>

| 영역 | 사용 경험 |
| :--- | :--- |
| **Backend** | Java · Spring Boot · Spring MVC · Spring Security |
| **Persistence** | JPA · QueryDSL · MyBatis · MySQL · MongoDB |
| **Frontend** | React · JavaScript · HTML · CSS · Thymeleaf |
| **Real-time** | WebSocket · STOMP · Redis Pub/Sub |
| **Infra & Delivery** | Linux · AWS EC2 · Amazon S3 · Docker · GitHub Actions |

<br>

## `04` / ENGINEERING NOTES

프로젝트에서 직접 고민하고 구현한 주제입니다.

| 주제 | 경험 |
| :--- | :--- |
| **Personalization** | 표본 수와 신뢰도를 반영한 단계별 추천 로직 |
| **Data Consistency** | 외부 AI 호출과 저장 단계 분리, 일기·추천의 원자적 저장 |
| **Observability** | 요청·응답·처리 시간·실패 단계 기록 |
| **Connection Lifecycle** | 인증 확인, 연결 복구, 종료 중 소켓 전송 제어 |

<br>

## `05` / LEARNING LOG

| 학습 주제 | 관심 방향 |
| :--- | :--- |
| **SQLD** | 데이터 모델링 · SQL 이해 |
| **FastAPI** | Python 기반 API 개발 |
| **LLM** | 프롬프트 · 응답 검증 · 서비스 적용 |

<details>
<summary><b>작은 프로젝트로 익힌 것들</b></summary>

<br>

| 프로젝트 | 학습 기술 |
| :--- | :--- |
| Emotion Diary | React |
| SNS | Spring Boot |
| Bulletin Board | Java · Database |

</details>

<br>

---

<div align="center">

### 새로운 서비스를 만들고, 더 나은 동작을 고민합니다.

**[GitHub](https://github.com/ohnuj) · [Gmail](mailto:jjh980225@gmail.com) · [Naver Mail](mailto:jjho980225@naver.com)**

<br>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,55:123D35,100:36D399&height=100&section=footer" alt=""/>

</div>
