<div align="center">

# JUNHO JANG
### Backend Developer · Java & Spring

**기능 구현부터 배포 후 문제 해결까지, 서비스의 전체 흐름을 고민합니다.**

Java와 Spring 기반으로 웹 서비스를 개발합니다.  
React 화면과 API를 연결하고, 실시간 통신·인증·데이터 처리 과정에서  
사용자가 겪는 문제를 찾아 개선하는 데 관심이 있습니다.

<br>

[![Gmail](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:jjh980225@gmail.com)
[![Naver Mail](https://img.shields.io/badge/Naver_Mail-03C75A?style=flat-square&logo=naver&logoColor=white)](mailto:jjho980225@naver.com)

</div>

<br>

## About Me

- **Backend 중심 개발** — Spring 기반 API와 데이터 처리, 인증·인가 및 서비스 로직 구현
- **사용자 흐름을 고려한 구현** — React 화면부터 API·DB까지 연결해 기능 완성
- **실시간 서비스 경험** — WebSocket·STOMP 및 Redis Pub/Sub을 활용한 채팅 구현
- **배포 이후의 문제 해결** — 브라우저 요청과 서버 로그를 바탕으로 인증·연결·파일 접근 문제 분석

<br>

## Selected Projects

| 프로젝트 | 소개 | 주요 기술 |
| :--- | :--- | :--- |
| **SPOILOCK** | 시청 진도 기반 AI 스포일러 보호 커뮤니티 | Spring Boot · React · Redis · WebSocket · FastAPI |
| **지구비우기** | 재활용 정보와 에코포인트를 연결한 친환경 실천 플랫폼 | Spring MVC · MyBatis · MySQL · Thymeleaf |
| **Mood & Move** | AI 감정 분석 및 맞춤형 행동 추천 서비스 | Spring Boot · React · MySQL · MongoDB · Gemini API |

<br>

### 01. SPOILOCK
> 시청한 만큼 이야기하고, 아직 보지 않은 이야기는 보호하는 드라마 커뮤니티

사용자별 시청 진도와 AI 판정 결과를 바탕으로 채팅·커뮤니티의 스포일러 노출을 제어하는 서비스입니다.  
드라마 시청, 실시간 채팅, 게시글과 댓글을 하나의 서비스 흐름으로 연결했습니다.

#### 서비스 주요 기능

| 영역 | 구현 내용 |
| :--- | :--- |
| 콘텐츠 | 작품·회차 조회, 영상 재생, 이어보기, 시청 진도 및 별점 관리 |
| 실시간 채팅 | 작품별 토론방·자유방·비밀방, 참여·퇴장, 방장 위임, 강퇴 및 초대 |
| 스포일러 보호 | AI 분석 결과와 작성자·조회자의 시청 진도를 반영한 공개 정책 |
| 커뮤니티 | 게시글·댓글, 전체 공개·팔로워 공개, 사진 첨부, 좋아요 및 팔로우 |
| 사용자 기능 | 마이페이지, 신고, 알림 및 읽지 않은 알림 수 표시 |
| 관리자 | 콘텐츠 관리, AI 판정 모니터링, 저작권 이용 권한·증빙자료·변경 이력 관리 |

#### 주요 담당 및 기여

- WebSocket·STOMP 기반 실시간 채팅과 채팅방 관련 기능 구현
- 참여자 접속 상태, 방장 위임, 초대 및 강퇴 등 채팅방 이용 흐름 구성
- 영상 시청·작품 상세·마이페이지 구현 및 화면과 API 연동
- 신고·팔로우 알림과 읽음·삭제 처리 구현
- 커뮤니티 사진 첨부와 미리보기, 공개 범위 및 수정·삭제 UI 개선
- 인증 복구 실패 시 반복 요청 제한과 WebSocket 연결·종료 처리 보완
- 관리자 저작권 이용 권한 및 증빙자료 관리 기능 구현

#### 기술적으로 고민한 부분

| 주제 | 접근 방식 |
| :--- | :--- |
| 서버 간 실시간 이벤트 전달 | Redis Pub/Sub을 통해 여러 Spring 서버에 이벤트 공유 |
| 인증 만료와 자동 조회 | 세션 복구 요청 공유, 실패 상태에 따른 요청 제한 및 재시도 |
| WebSocket 연결 수명 관리 | 연결 전 인증 확인, 중단된 연결 복구, 화면 종료 시 자원 정리 |
| 스포일러 공개 정책 | AI 판정과 실제 공개 여부를 분리하고 사용자별 시청 진도 반영 |
| AI 판정의 한계 | 회차 정확도·인터넷 표현·동일 입력의 일관성 문제를 정리하고 개선 방향 검토 |

**Tech Stack**

`Java` `Spring Boot` `Spring Security` `JPA` `QueryDSL` `MySQL`  
`React` `Redis` `WebSocket` `STOMP` `FastAPI` `Gemini API`  
`AWS EC2` `Amazon S3` `GitHub Actions`

<sub>프로젝트 전체 기술 스택이며, 개인 담당 범위는 위의 ‘주요 담당 및 기여’에 구분했습니다.</sub>

<br>

---

### 02. 지구비우기
> 재활용 정보를 찾는 것에서, 직접 실천하는 경험까지

재활용 정보 검색과 수거함 위치 조회를 제공하고,  
커뮤니티 활동과 미니게임을 에코포인트·리워드 교환으로 연결한 친환경 플랫폼입니다.

| 영역 | 구현 내용 |
| :--- | :--- |
| 재활용 정보 | 공공데이터 기반 품목 검색 및 분류 기준·배출 방법 안내 |
| 에코맵 | Kakao Map 기반 수거함 위치 조회 및 종류별 필터링 |
| 에코포인트 | 활동별 포인트 적립·차감 및 변동 이력 관리 |
| 리워드 | 포인트 잔액·상품 재고 검증, 교환 신청 및 관리자 처리 |
| 커뮤니티 | 게시글·댓글, 공지사항 및 건의사항 |
| 참여 기능 | Drag & Drop 방식의 재활용 분류 미니게임 |

#### 주요 담당 및 기여

- 화면 흐름과 ERD 설계 및 데이터베이스 구성
- 재활용 정보 검색 기능 구현
- 에코포인트 적립·사용 및 이력 관리
- 리워드 교환과 관리자 처리 기능 구현
- 팀장으로서 역할 분담과 진행 상황 조율

**Tech Stack**

`Java` `Spring MVC` `MyBatis` `MySQL` `Thymeleaf` `JavaScript`

<br>

---

### 03. Mood & Move
> 감정 기록을 바탕으로, 지금 나에게 필요한 행동을 제안하는 서비스

사용자의 감정과 일기 내용을 분석하고 Gemini API를 활용해 행동을 추천합니다.  
행동 실행 후의 감정 변화와 사용자 선호 정보를 추천 개인화에 활용하도록 구성했습니다.

| 영역 | 구현 내용 |
| :--- | :--- |
| 감정 기록 | 감정·일기 입력 및 현재 상태 분석 |
| AI 추천 | Gemini API 기반 맞춤형 행동 제안 |
| 개인화 | 선호·비선호·취미 및 행동 실행 결과 반영 |
| 통계 | 감정 기록과 행동 효과 시각화 |
| 사용자 관리 | 인증 및 회원정보 관리 |
| 배포 | Docker·AWS EC2 기반 서비스 배포 |

**Tech Stack**

`Java` `Spring Boot` `JPA` `MySQL` `MongoDB`  
`React` `Gemini API` `Docker` `AWS EC2`

<br>

## Technical Skills

| 분야 | 사용 기술 |
| :--- | :--- |
| **Languages** | Java · JavaScript · Python |
| **Backend** | Spring Boot · Spring MVC · Spring Security · JPA · QueryDSL · MyBatis |
| **Frontend** | React · HTML · CSS · Thymeleaf |
| **Data** | MySQL · MongoDB · Redis |
| **Communication** | REST API · WebSocket · STOMP · Redis Pub/Sub |
| **Infra & Delivery** | Linux · AWS EC2 · Amazon S3 · Docker · GitHub Actions |
| **Tools** | Git · GitHub · IntelliJ IDEA · VS Code · MySQL Workbench |

<br>

## Engineering Focus

**실패한 이후의 흐름까지 설계하기**

요청 성공뿐 아니라 인증 만료, 연결 중단, 외부 API 지연 상황에서  
사용자에게 무엇을 보여주고 언제 다시 시도할지 함께 고민합니다.

**문제를 재현하고 근거로 확인하기**

브라우저 네트워크 요청, 서버 로그, 데이터베이스 상태를 함께 확인하며 원인을 좁힙니다.  
빌드 성공과 실제 서비스의 정상 동작을 구분하고, 수정 후에는 해당 흐름을 다시 검증하려고 합니다.

**AI를 서비스의 한 부분으로 다루기**

AI 응답을 그대로 사용하는 데 그치지 않고, 데이터 품질과 판정 근거,  
공개 정책, 지연과 비용까지 고려하는 개발을 지향합니다.

<br>

## Study & Practice

| 주제 | 학습 프로젝트 |
| :--- | :--- |
| React | Emotion Diary |
| Spring Boot | SNS |
| Java · Database | Bulletin Board |

<br>

---

<div align="center">

### Contact

프로젝트와 개발 경험에 대한 이야기를 환영합니다.

**[jjh980225@gmail.com](mailto:jjh980225@gmail.com)**  
**[jjho980225@naver.com](mailto:jjho980225@naver.com)**

</div>
