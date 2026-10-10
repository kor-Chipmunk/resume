# 김선재
제품 출시를 보장하는 5년차 Java / Spring Boot 서버 개발자입니다.  
글로벌 앱 서비스의 가상 재화와 이커머스의 실물 상품 재화를 관리했고,  
상품 노출 예약, 자동 발주, 구독 등 시간을 제어하는 시스템 구축 경력으로 지녔습니다.  
업무 품질을 높이기 위해 테스트 코드로 검증하고, 대시보드와 메트릭과 같은 데이터 기반으로 업무 완성을 검증합니다.

- Github: [kor-Chipmunk](https://github.com/kor-Chipmunk/)
- Blog: [itchipmunk](https://itchipmunk.tistory.com)
- Kakaotalk: chipmunks
- Email: rhj4862@gmail.com

## 목차
- [경력](#경력)
- [기술](#기술)
- [프로젝트](#프로젝트)

# 경력

## 회사

### [엔이피데이터(부스패치/복덕)](https://www.boospatch.com)
- 기간 : 26.04 ~ 현재
- 소속 : 기술 공동창업
- 부동산 현장감이 높은 데이터를 제공하고 막막한 내집마련을 도와주는 B2C 플랫폼 / 공인중개사의 매물 광고와 손님 관리 업무를 높은 품질로 자동화하는 B2B 플랫폼
- 사용 기술
  - Backend : Node.js / Spring
  - Frontend : React
  - Infra : PostgreSQL, AWS SQS, DataDog, Docker, AWS
- 협업 도구 : Git, Slack, Notion
- 경험
  - SQS / Transactional Outbox / LLM 통신 안정화 / 단건 결제 기반 개인화 부동산 리포트 시스템 구축
  - 정기 결제 / 콘텐츠 메일링 시스템 구축
  - 추천 유입 및 출판사 협업 위한 쿠폰 시스템 구축
  - 데이터 파이프라인 / 서빙 레이어 구축
  - 유저 행동 로그 수집 / 서비스 지표 및 퍼널 대시보드 구축

### [푸드팡](https://foodpang.co/)
- 기간 : 24.05 ~ 26.04
- 소속 : 개발팀 - 풀필먼트
- 16,000명의 외식업 사장님께서 사용하는 식자재 새벽 배송 B2B 플랫폼
- 사용 기술
  - Backend : Spring Boot, Spring Batch, jOOQ, Java, Kotlin
  - Frontend : Vue.js, Pinia, Vite
  - Infra : MariaDB, Apache Kafka, Jenkins, Telegraf, Prometheus, Loki, Grafana, Docker, AWS
- 협업 도구 : Git, Slack, Asana, Notion, Gitea
- 경험
  - PMS(구매 관리 시스템) REST API / Batch / Event / Admin : 개발 / 배포 / 운영 담당
  - 코틀린 기반 PG사 결제 연동 SDK 개발
  - 실무자 시세 구글시트 API 연동, GAS 코드 지원으로 실데이터 기반 검수 지원
  - OMS(주문 관리 시스템) 거래명세서 엑셀을 작성하는 Apache POI 컴포넌트 고도화로 사진 첨부, 수식 작성, 셀 병합 지원
  - 브랜드 통합 공지사항 관리 고도화 & 구매 이력 기반 상품 판가 하락 푸시알림 배치 & A/B 테스트 시스템 구축
  - Gitea / Telegraf / Prometheus / Loki / Grafana 등 인프라 관리
  - 배치 스크립트로 운영 업무 지원 - 보고서, 시트, 알림 등


### [와이피랩스(커넥팅)](http://connectingapp.co.kr/)
- 기간 : 20.10 ~ 22.12 (2년 3개월, 병역특례)
- 소속 : 프로덕트팀
- 200만 유저 규모의 다국가 소셜통화 앱 서비스 스타트업으로 IMM 인베스트먼트 등으로부터 100억 시리즈B 투자 유치
- 사용 기술
  - Backend : Django, DRF(Django Rest Framework), NestJS, WebSocket, Python, TypeScript
  - Frontend : Vue.js
  - Infra : MySQL, Redis, AWS EB, AWS ECS, Docker
- 협업 도구 : Git, Slack, Jira Confluence, Notion
- 경험
  - 앱 서비스의 **REST API / WebSocket 서버** 개발 / 배포 / 운영
  - 기존 레거시 확장 비용이 높아, 신규 WebSocket 매칭 서버 **1인 구축**
  - 시리즈B 유치를 위한 매출 증대 목적으로, 인앱 구독 결제 연동 시스템 **1인 구축**
  - 안정적이고 빠른 출시를 위해, CI 실행 시간 **42% 개선** / 테스트 커버리지 **0% → 80% 달성**

# 기술

## Java / Spring
실무 경험 (MariaDB / Apache Kafka)
- **Batch** : 실시간 예약 배치 시스템 설계 / 개발 / 운영
  - 분산 비동기 스케쥴러 JobRunr 활용으로 분산 배치 시스템 구축
  - 동시 실행으로 인한 DeadLock / HikariCP 고갈 현상 수정 : 트랜잭션 격리 수준 / ReentrantLock & Semaphore

**3개**의 팀프로젝트 기술 리드 경험 (Spring Boot / JWT / JPA / Docker)
- **ORM** : **생산성**을 위해 간단한 쿼리는 JPA, 복잡한 Join / 동적 쿼리는 QueryDSL 채택

## Django / DRF
2년간 실무 경험 (MySQL8 / Redis)
- **ORM**
  - DB Join 비용과 개별 쿼리 매핑 비용을 비교해 **쿼리 속도 개선**
  - 도메인 / 쿼리 로직을 분리해 **중복 코드 제거**, **테스트 가독성**, **유지보수성**을 높임
- **Batch** : **100만 단위** 데이터를 **Chunk 단위 Bulk** 배치 작성
- **Lock** : Redis 분산 락으로 멀티 프로세스 동시성 제어

## Node.js / NestJS
**1년간 실무** 경험 (WebSocket / Redis)
- **비동기** : **성능 향상**을 위해, 불필요한 await 제거 / Promise.all() 으로 네트워크 I/O 개선
- **동시성** : 동시성 큐로 대화방 입장 / 마감 처리

# 프로젝트

## 경력 프로젝트

### 구매 이력 기반 상품 판가 하락 푸시알림 배치 & A/B 테스트 시스템 구축

- 기간 : 2026.02 ~ 2026.03 (2개월)
- 성과
  - 대조군 대비 주문 단가 20% 상승
- 역할
  - 기획자와 데이터 분석 지원
    - 기존 기획의 푸시알림 대상자가 극히 적어 실효성을 부정 -> B2B 고객을 감안해 구매 이력 기반과 주문 주기 기반을 제안
    - 주문 주기는 딥링크 선행 개발이 필요해 빠르게 구현할 수 있는 구매 이력 기반으로 결정
    - 대상 선정을 위한 지표를 확인할 수 있는 그라파나 대시보드를 구축해 기획자에게 전달
  - 마케팅이 아닌 서비스 팀의 푸시 알림 기획은 처음으로 보수적으로 접근 유도
    - 고객의 푸시 알림 반응 데이터가 없기에 처음 기획부터 푸시 알림을 차단하는 불상사를 방지하기 위함
    - A/B 테스트 시스템을 구축해 실험군과 대조군을 매일 배치로 선정하여 푸시알림을 전송하도록 결정
  - 대상자 선정과 푸시알림 발송 시점을 분리하여 조건 선검수 후 푸시알림을 발송하도록 결정
  - 성과 측정 위해 사용자 여정을 파악하는 앰플리튜드 대시보드 구축 / 구글 애널리틱스 푸시알림 지표 대시보드 구축
    - iOS 푸시알림 업데이트 버그와 안드로이드 앰플리튜드 이벤트 미연동 건 클라이언트 개발자에게 이슈업하여 수정
- 기술
  - Spring Boot

### 시세 업데이트 자동화 시스템 설계 및 구현

- 기간 : 2025.12 ~ 2026.01 (2개월)
- 성과
  - 실무자 작업 시트내 실제 시세 정합성을 주기적으로 검증해 잘못된 마진으로 게시 중인 상품 목록을 메신저 경보로 알려 매출 손해 방지
  - 외부 인프라의 한계를 극복하여 사내 시스템과 통합 : GAS 실행시간 제한으로 트리거 역할로 고정, 시간이 오래 걸리고 무거운 연산은 서버에서 처리
  - A1 표기법 기반의 구글 시트 DSL 설계하여 이기종 시트를 단일 추상화로 처리
  - Google API 제한량 대응 : Spring Retry 적용하여 배치 스케쥴러에서 대량 셀 읽기 / 쓰기시 API 제한에 따른 분단위 재시도로 로직 정상 수행 / 배치 API 사용으로 API 호출 횟수 최소화
  - 안정적인 GAS 코드 지원 : 10여개 시트 갱신 감지시 GAS 30초 실행 타임아웃 제약을 해결하기 위해 캐싱 API 사용
  - 스냅샷 기반 아키텍처로 상태 머신으로 데이터 정합성 보장하고 중복 처리 방지
  - 구글에서 제공하는 clasp 도구로 GAS 프로젝트 코드 형상 관리, 스크립트 실행으로 자동 배포 환경 구성
- 기술
  - Server : Spring Boot
  - GAS : JavaScript, clasp

### jOOQ 연관 컬렉션 내부 기능으로 인한 페이지네이션 쿼리 성능 저하 개선

- 기간 : 2025.10
- 성과
  - 4초 내외의 페이지네이션 쿼리를 0.3초로 단축
- 역할
  - jOOQ 내 컬렉션 객체로 연관 테이블을 포함시켜주는 multiset 함수의 내부 동작은 상관 서브쿼리와 JSON_ARRAY를 조합
  - LIMIT / OFFSET 쿼리의 한계로 사용하지 않는 Row 를 연산함으로써 성능 저하 발생한다고 추정
  - SQL Explain 시 임시 테이블 쓰기로 파악
  - MariaDB와 연동한 Telegraf 에서 수집한 지표를 바탕으로 Grafana에서 임시 테이블 생성율, 디스크 임시 테이블 생성율 지표
가 치솟는 현상 확인
  - 페이지에 해당하는 쿼리를 서브쿼리로 분리하고 인덱스 스캔만 진행한 다음, 해당하는 Row Id만 multiset 함수 로직이 적용되도
록 수정
- 기술
  - Spring Boot, Grafana

### 본사 및 공급처 담당자용 발주 업무 시스템 개발

- 기간 : 2025.03 ~ 2025.08 (6개월)
- 성과
  - 주문, 재고, 배차, 알림 시스템과 연동한 발주 업무 시스템 개발
- 역할
  - 특정 시간대마다 실시간으로 변경되는 데이터를 API로 조회해 스냅샷 데이터 갱신 및 발주 원장(Ledger)으로 적재
  - 목킹한 JSON 응답과 테스트 데이터베이스 데이터, 시간 목킹으로 인수 테스트 코드 40여개 작성
  - SQL / Grafana로 타시스템의 데이터베이스와 Grafana Transform Join으로 연동해 수량 정합성 검증 대시보드 구축
    - 주문은 원장 방식이 아니라, 상태 기반이기에 스냅샷 이후 주문 취소로 인한 오차 존재
    - 주문 취소 테이블 연동 / 주문 수량을 모두 취소해 주문 Row가 사라진 경우는 발주 데이터와 비교해 취소 수량 추적
  - 알림톡 발송하는 사내 메시징 시스템 유지보수 / 개발 환경 위한 휴대폰번호 화이트 리스트 규칙 제안해 컴포넌트 개발 및 테스트 코
드 작성
- 기술
  - Spring Boot, Vue.js, MariaDB, Apache Kafka

### PG사 결제 연동 SDK 개발

- 기간 : 2024.11 ~ 2024.11 (1개월)
- 성과
  - 기존 PG사 현금흐름 지원 정책 중지에 빠르게 대응
  - 엄격한 객체와 테스트 코드 작성의 결과로 PG사 문서의 내용이 실제 요청과 일부 다른 점(필드명 오타, 누락된 데이터)이 있어 취합 후 사내 공유
- 역할
  - 업무가 몰린 서비스팀 개발 지원 / PG사 결제 연동 라이브러리 개발 (총 1인 담당)
  - 코틀린 기반 커머스 시스템을 지원하기 위해 코틀린으로 개발 언어를 확정
  - Ktor HttpClient 코드를 모방해, 수신 객체 지정 람다 기반 DSL 형식으로 진입 객체 설정을 편리하게 구현
  - 코루틴 구조로 설계해 I/O 처리 효율을 높이고, 코루틴을 지원하지 않는 시스템을 위해 `runBlocking` 으로 감싼 `XXXSync()` API를 지원
  - 람다 함수가 객체로 변환되지 않아 성능상 이점이 있는 인라인 함수를 적극 사용하고, 객체 변환 없이 필드값으로 대체하는 인라인 클래스로 리팩터링
  - 비즈니스 처리를 엄격히 만들기 위해, PG사에서 오는 요청의 모든 값을 값 객체로 만들어 문서대로 검증하는 객체 구조로 처리
  - Kotest 테스트 프레임워크로 170개의 테스트 코드를 작성 / 테스트 코드의 성능을 증가시키기 위해 파일 단위와 Spec 테스트 단위로 병렬 설정 추가
  - `runCatching` / `Result` 으로 성공과 오류를 구분하고, 오류 핸들링을 클라이언트에게 위임
  - 민감 정보 마스킹 처리 및 로그 적재 / 프로메테우스 결제 메트릭 수집 모듈 개발
- 기술
  - 언어 : Kotlin
  - 라이브러리 : Ktor HttpClient, kotlin-coroutine, Micrometer
  - 테스트 프레임워크 : Kotest
  - 배포 : Nexus Repository

### 상품 관리 예약 배치 시스템

- 기간 : 2024.07 ~ 2024.10 (1개월 개발 / 3개월 유지보수)
- 성과
  - 야간 무인 운영으로 인건비 감소
  - 발주 시간 75% 감소
- 역할
  - PMS(구매 관리 시스템) REST API / Batch / Event / Admin 개발 (총 2인 담당)
  - 배치 동시 실행으로 인한 DeadLock / HikariCP 커넥션 고갈 문제, 트랜잭션 격리 수준 / Locking 기법으로 해결
  - 장애 전파를 막기 위한 Fault Tolerance 시스템 구축 (모니터링 알람 / Retry 전략 수립)
  - 커넥션풀 메트릭을 포함한 스프링 애플리케이션 대시보드 / 예약 건 추적을 위한 그라파나 대시보드 구축
  - 야간 배치 모니터링 / 온콜 대응
- 기술
  - 서버 : Java, Spring Boot, Spring Batch, jOOQ
  - 어드민 : Vue.js, Pinia
  - 인프라 : MariaDB, Apache Kafka, Jenkins, Grafana, Prometheus

### Agora SDK 기반 음성 데이터 적재 파이프라인 및 CS 위한 음성 플레이어 개발

- 기간 : 2022.11
- 성과
  - 데이터 분석 위해 사내 구축 플랫폼에서 Agora SDK로 이전, 1TB 상당의 음성 데이터 확보
  - 짧은 만료시간의 S3 Presigned URL 음성 파일 다운로드로 보안성을 챙긴 HLS 플레이어 컴포넌트 개발
- 역할
  - Agora SDK 음성 통화 녹음 및 웹훅 연동
  - CS 대응 어드민에 적재한 음성 통화를 들을 수 있는 HLS 플레이어 컴포넌트 추가
- 기술
  - Django, Vue.js

### 국가간 채팅 기능 개발

- 기간 : 2022.10 ~ 2022.11 (2개월)
- 성과
  - 한국/일본 2개국 기능 출시
- 역할
  - REST API 개발 1인 담당 ( 담당자 서버 2인, 모바일 1인 )
  - SaaS 메타데이터에 Type 을 정의해 기존 메신저 기능을 실시간 채팅으로 확장 / API 연동 확장
  - 네트워크 호출 안정성을 위해, 흩어진 네트워크 호출 코드를 네트워크 모듈로 리팩터링 / 기본 TimeOut 설정
  - CS 업무 지원 / 웹 어드민 인력 지원 위해, 채팅 내역 조회 무한 스크롤 컴포넌트 작성
- 기술
  - Django, Vue.js

### 인앱 구독 결제 연동 시스템 구축

- 기간 : 2021.03 ~ 2021.04 (2개월)
- 성과
  - 매출 증대로 시리즈B 투자 유치에 기여
- 역할
  - 앱스토어 / 플레이스토어 구독 연동 시스템 1인 구축 ( 담당자 서버 1인, 모바일 1인 )
  - 구독 상태 / 구독 상품을 위한 15개 데이터 모델링 / REST API / Django Admin 개발
  - 스토어 콜백 가용성 보장과 메시지 유실을 방지하기 위해, 클라우드 서버리스 채택  / 클라이언트측 재검증 로직 협의
  - 100만 단위 초기 데이터 Bulk Insert 배치 개발
- 기술
  - Django, GCP Pub/Sub & Cloud Function

### 그룹 통화 기능 개발 & 운영

- 기간 : 2021.08 ~ 2022.12 (1년 5개월)
- 성과
  - 베타테스트 이후 장애 없이 일일 평균 2,000 건 이상 매칭 처리
- 역할
  - 신규 기능을 검증하기 위해 REST API / 웹소켓 매칭 서버 1인 구축 ( 담당자 서버 1인, 모바일 1인 )
  - 매칭 순서 보장 / 동시성 방지 위한 인메모리 작업 큐를 도입하고 Redis 큐로 모듈 확장
  - 배포 자동화 구축을 위해, 컨테이너 기반 AWS ECS Fargate 에 배포하는 Github Actions 워크플로우 구축
- 기술
  - Django, NestJS, WebSocket, Redis, AWS ECS

### 테스트 코드 개선

- 기간 : 2021.06  ~ 2022.11 (1년 6개월)
- 성과
  - CI 실행 시간 7분 → 4분 (42%) 단축하여 배포 시간 단축
  - 테스트 실행시간 300s → 150s (50%) 단축하여 생산성 증대
  - 테스트 커버리지 0% → 80% 달성으로 기존 비즈니스 로직 동작 보장
- 역할
  - 6~7분의 CI 시간이 빠른 배포에 악영향을 끼쳐, Github Actions matrix 병렬처리로 42% 단축
  - 유닛 테스트 / 외부 API 목킹과 데이터 픽스처로 테스트 시간 단축 (60% 기여)
  - 레거시 안정성을 보장하기 위해, 통합 테스트 작성 후 유닛 테스트로 테스트 커버리지 보충 (60% 기여)
- 기술
  - pytest, pytest-split, Github Actions

## 개인 프로젝트

### 음원 스트리밍 플랫폼

스마일게이트 개발캠프에서 1개월간 진행한 서버 3인/웹 1인으로 구성된, Spring MSA 프로젝트입니다.

- 기간 : 2024.01 ~ 2024.02
- 소속 : 스마일게이트 개발캠프 5기
- 역할
  - 백엔드 기술 리드. 개발 이슈(일정관리/디버깅) 해결, 외부 커뮤니케이션 지원
  - 음원 전처리 후 WebSocket 으로 스트리밍 개발, MVC -> WebFlux 구조로 32% 전체 다운로드 시간 개선
  - 서비스 디스커버리 / 게이트웨이 라우팅 패턴으로 게이트웨이 서버 구축
  - 멀티 모듈 / 전체 서비스 공통 모듈 구축
  - 도커 인프라 구축 (15개 서비스와 Kafka 인프라 도커 구축 / 포트 및 환경 변수 정리)
- 기술 : Spring Boot, JPA, Spring Cloud, Docker
- 링크
  - 깃허브 : https://github.com/sgdevcamp2023/sgwannabe

### 운동 대회 플랫폼

대학생 운영 대회와 친선 교류전을 개최하는 서비스입니다.

- 기간 : 2023.07 ~ 2023.09
- 소속 : UMC
- 역할
  - 백엔드 기술 리드
    - DB ERD 22개 테이블 설계 ([링크](https://itchipmunk.tistory.com/565))
    - 팀원을 위한 프로젝트 코드 컨벤션 설정 ([링크](https://itchipmunk.tistory.com/576))
  - REST API 25개 엔드포인트 구현 (기여도 60%)
  - AWS 인프라 구축
    - MFA 기반 IAM 팀원 계정 관리 ([링크](https://itchipmunk.tistory.com/550))
    - AWS EC2, RDS, S3, CloudFront, Route53 인프라 구축
    - Github Actions, AWS CodeDeploy 으로 EC2 배포 자동화 구축
- 기술 : Java, JPA / QueryDSL, JWT
- 링크
  - 깃허브 : https://github.com/HUSTLE-UMC/HUSTLE_server

### 함께 만드는 플레이리스트, 뮤즐리 (서비스 종료)

노래 플레이리스트를 사람들과 공유하는 서비스입니다. 

- 기간 : 2022.06 ~ 2022.09
- 소속 : 매쉬업
- 역할
  - 3개의 페이지와 1개의 QR 컴포넌트 작성
  - 전체 13개 API 호출 훅 추가
  - CI 워크플로우와 랜덤 리뷰어 워크플로우 적용
- 기술 : TypeScript, React.js, NextJS, StompJS
- 링크
  - 깃허브 : https://github.com/mash-up-kr/muzily-web

![image](https://user-images.githubusercontent.com/16275188/211581593-03d6bb87-31f9-4102-912b-c4bcd249481f.png)


### 나들길 (서비스 종료)

주변 산책 길을 저장하고 다른 사람들과 공유할 수 있는 커뮤니티 프로젝트입니다.  
NodeJS 환경의 NestJS 프레임워크와 TypeORM 라이브러리를 사용했습니다.  
PostgreSQL의 지리 기능 중 열린 직선들을 저장할 수 있는 데이터 타입으로 산책길 정보를 저장해보는 경험을 해보았습니다.  
행정동 데이터를 외부에서 가져와 DB에 저장하고 위치 기반으로 주변 행정동 데이터를 조회해보는 경험을 해보았습니다.  

- 기간 : 2021.09 ~ 2021.12
- 소속 : 매쉬업
- 역할 : Backend
- 사용기술 : NodeJS, TypeScript, NestJS, TypeORM
- 링크
  - 깃허브 : https://github.com/mash-up-kr/HikingClub_Node

![Onboarding_main](https://user-images.githubusercontent.com/16275188/173311604-ff7095ff-de0a-4bea-ae52-9010d1440aa1.png)
![홈 리스트](https://user-images.githubusercontent.com/16275188/173311613-fa2e2d51-81af-42db-ba09-23ab890eddc3.png)
![길 상세 -1- 내가 쓴 글](https://user-images.githubusercontent.com/16275188/173311684-e303ac2d-c258-4de1-a566-984e28c1add5.png)
![길 등록 - 카테고리_2](https://user-images.githubusercontent.com/16275188/173311887-988e183e-2e25-41da-abc4-8db1a1b6620d.png)



### 신비로운 동물 상담소 (서비스 종료)

위치 기반 고민 상담 커뮤니티 프로젝트입니다.  
NodeJS 환경의 Express 라이브러리를 사용하여 백엔드 서버를 개발했습니다.  
MySQL에서 제공하는 지리 SQL로 반경 N km 에 위치하는 데이터를 조회하는 경험을 해보았습니다.  

- 기간 : 2021.02 ~ 2021.05
- 소속 : 매쉬업
- 역할 : Backend
- 사용기술 : NodeJS, express, sequelize, pm2, redis, aws
- 링크
  - 깃허브 : https://github.com/mash-up-kr/CowCat_Node

![KakaoTalk_Photo_2021-05-08-05-43-41 1](https://user-images.githubusercontent.com/16275188/173309573-adf4ca2f-f0b7-4dda-94dc-0c14a4b3dfd0.png)
![KakaoTalk_Photo_2021-05-08-05-37-31 1](https://user-images.githubusercontent.com/16275188/173309609-f7a1095c-c45c-4b34-a208-b3e3f7dd765b.png)
![KakaoTalk_Photo_2021-05-08-05-37-20 1](https://user-images.githubusercontent.com/16275188/173309701-af1f93b6-4e60-42bb-94c3-892d371ba3d9.png)
![KakaoTalk_Photo_2021-05-08-05-37-28 1](https://user-images.githubusercontent.com/16275188/173309723-18526071-75dd-4342-89c2-11894ddf8010.png)


### 모각공 - 모여서 각자 공부 (서비스 종료)

공부시간을 측정하고 다른 이들과 공부시간을 경쟁하는 프로젝트입니다.  
스프링 부트로 데이터베이스 테이블 설계와 REST API를 설계해 볼 수 있었습니다.
스프링 부트 개발부터 AWS EC2 & CodeDeploy 자동화 배포까지 경험해볼 수 있었습니다.  

- 기간 : 2020.07 ~ 2020.09
- 소속 : 매쉬업
- 역할 : Backend
- 사용기술 : java 8, Spring boot 2, jpa, redis, nginx, aws
- 링크
  - 깃허브 : https://github.com/mash-up-kr/Dionysos-Backend

![images](./images/mogakgong1.png)

### MOTI (~25.04.18 서비스 종료)

매일 새로운 질문으로 나만의 드림캐처 만들기 서비스입니다. 가장 최근 기술인 SwiftUI를 사용한 프로젝트입니다.  
기타 라이브러리는 Moya, Alamofire, Kingfisher 입니다.  
제플린으로 디자이너와 협업하고 Swagger 로 백엔드와 협업하고 노션으로 일정과 QA를 관리했습니다.

- 기간 : 2019.12 ~ 2020.05
- 소속 : 매쉬업
- 역할 : iOS, Backend
- 주 업무 : SwiftUI 뷰 개발, 네트워크 레이어 개발
- 사용기술 iOS : Swift5, SwiftUI, Moya, Alamofire, Kingfisher
- 사용기술 Backend : NestJS, Typescript
- 링크
  - iOS 깃허브 : https://github.com/mash-up-kr/Ahobsu_iOS
  - Backend 깃허브 : https://github.com/Yuni-Q/moti-backend
  - 앱스토어 : https://apps.apple.com/kr/app/moti/id1496912171
  - 홈페이지 : https://his-0203.github.io/
  
![images](./images/moti1.png)

### AllNight (서비스 종료)

칵테일러들을 위한, 칵테일 레시피를 알려주는 서비스입니다.  

- 기간 : 2019.6 ~ 2019.9
- 소속 : 매쉬업
- 역할 : iOS
- 주 업무 : 칵테일 상세 뷰 개발
- 사용기술 : Swift, Moya, Kingfisher, SwiftLint, SwiftyBeaver
- 링크
  - 깃허브 : https://github.com/mash-up-kr/AllNight-iOS

### PerfectPitch

영상처리 과목 프로젝트 결과물입니다. 디지털 악보의 박자, 마디, 음표를 인식해 피아노로 연주하는 프로젝트입니다.

- 기간 : 2018.11
- 소속 : 중앙대학교
- 역할 : C++ MFC UI 프로그램 개발, 코어 API 개발
- 주 업무 : C++ MFC UI 프로그램 개발
- 보조 업무 : Core API 중 Binarization, Detecting five lines 개발
- 사용기술 : C++, OpenCV
- 링크
  - 깃허브 : https://github.com/kor-Chipmunk/PerfectPitch-UI

### Code Name : Seoul (서비스 종료)

모바일 웹 방탈출 게임 서비스입니다. 아이디어 기획부터 컨텐츠 답사, 배포까지 해 본 소중한 경험이었습니다.  
루비온레일즈 MVC패턴으로 구성하고 AWS Route53으로 도메인 호스팅까지 해 본 프로젝트입니다.

- 기간 : 2017.07 ~ 2017.08
- 소속 : 멋쟁이 사자처럼
- 역할 : Backend
- 사용기술 : Ruby on Rails 5, aws s3, aws ec2, aws route53
- 링크
  - 깃허브 : https://github.com/kor-Chipmunk/code_name_seoul

![images](./images/codename1.png)
![images](./images/codename2.png)
![images](./images/codename3.png)

## 단체
- 매쉬업
  - 기간 : 18.03 ~ 22.12
  - 디자이너와 개발자가 함께하는 모바일 앱 개발 IT 동아리입니다.
  - 개발자 / 디자이너분들과의 네트워킹과 사이드 프로젝트를 진행합니다.
  - 블로그 : https://mash-up.tistory.com/
  - 회고록 : https://itchipmunk.tistory.com/488
- CUAI
  - 기간 : 2019.03 ~ 2019.12
  - 중앙대학교 빅데이터 동아리입니다. 머신러닝과 딥러닝 세션을 진행합니다. 자체 컨퍼런스를 진행하고 여러 경진 대회에 참가합니다.
  - 블로그 : http://blog.naver.com/cuaibigdata
  - 회고록 : https://itchipmunk.tistory.com/422
- 멋쟁이 사자처럼
  - 기간 : 16.03 ~ 17.08
  - 다양한 배경의 학생들이 모여 IT 웹 서비스를 런칭하는 동아리입니다.
  - 모교 운영진으로 Ruby on Rails와 HTML/CSS/JS 교육을 주도하는 역할을 맡았습니다.
  - 회고록 : https://itchipmunk.tistory.com/91

## 학교
- 중앙대학교 : 2016.03 ~ 2023.08
  - 주전공 : 전자전기공학부
  - 복수전공 : 컴퓨터공학부
- 한국디지털미디어고등학교 : 2013.03 ~ 2016.01
  - 전공 : 해킹방어

## 수상 

### 재생에너지 발전량 예측 경진대회 장려상

풍력 분야 발전량 예측 분야에서 장려상

- 기간 : 2019.07 ~ 2019.08
- 주최 : 전력거래소

### 전력데이터 신서비스 개발 경진대회 우수상

한국전력에서 주관하는 전력데이터를 활용한 신서비스 개발 경진대회에서 '소상공인을 위한 컨설팅 서비스'를 출품

- 기간 : 2019.03
- 주최 : 한국 전력
