# 안녕하세요, 구본상입니다

> 당장의 구현보다, **오래 갈 수 있는 선택**을 하는 백엔드 개발자입니다.

금융권 SI 환경에서 4년간 K-Bank, 카카오뱅크 등 금융 시스템 고도화 프로젝트를 수행했습니다.<br>
기능을 빠르게 만드는 것보다, **기준을 세우고 구조를 잡아 재작업을 줄이는 방식**으로 일해왔습니다.

<br>

## 🛠️ Tech Stack

**Back-end**
<p>
  <img src="https://img.shields.io/badge/Java_17-007396?style=flat-square&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/Spring_Boot_3.x-6DB33F?style=flat-square&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/MyBatis-C4A764?style=flat-square&logoColor=white">
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white">
</p>

**Database & Infrastructure**
<p>
  <img src="https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white">
  <img src="https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white">
</p>

**Front-end & Tools**
<p>
  <img src="https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white">
</p>

<br>

## 💼 Career

| 기간 | 소속 | 직무 |
|------|------|------|
| 2022.03 – 2025.12 | 로이솔루션 (SI 개발팀) | 웹/백엔드 개발자 · 대리 |

금융권 회계·예산·IFRS 시스템 고도화 프로젝트를 주로 수행했습니다.<br>
초기부터 화면·배치·인터페이스를 포괄하는 풀사이클 개발을 담당했고,<br>
프로젝트 후반부에는 공통 설계와 데이터 기준 정립을 주도했습니다.

<br>

## 📌 Key Projects

### K-Bank IFRS 시스템 고도화 | 2025.04 – 2025.12

> `Java 17` `Spring Boot 3.x` `MyBatis` `Oracle` `Vue 3`

**대용량 엑셀 다운로드 안정화**
- 100만 건 이상 결산 데이터 추출 시 힙 메모리 병목 문제 해결
- SXSSF(Streaming XSSF) 도입으로 일정 행만 메모리 유지, 초과 데이터 디스크 Flush 처리
- 20만 건 단위 분할 다운로드 + 상위 200행 샘플링 기반 컬럼 너비 산출로 서식 요건 충족

**공통 페이징 구조 설계**
- 조회·엑셀 SQL 이원화로 인한 정합성 불일치 리스크를 MyBatis Interceptor 기반 구조로 해결
- 동일 SQL을 컨텍스트(화면/엑셀)에 따라 페이징 동작만 분기 → 신규 메뉴 개발 속도 약 30% 단축

**인증·권한 체계 설계**
- JWT 즉시 무효화가 어려운 리스크를 고려, 서버 통제 가능한 세션 기반 인증 방식 선택
- 중복 로그인 방지, 세션 자동 만료, RBAC 메뉴 접근 제어 구현 → 보안 심의 무결함 통과

---

### 카카오뱅크 예산자산 시스템 고도화 | 2023.11 – 2024.11

> `Java 17` `Spring Boot 3.x` `MyBatis` `Oracle` `Vue 3`

**경비집행 도메인 구조 설계**
- 검증 요건 변경이 잦은 환경에서 결재 흐름을 검증 / 계산 / 외부 연동 단계로 명확히 분리
- 단계별 검증 로직을 함수 단위로 모듈화 → 변경 시 해당 모듈만 수정하는 구조 확보

**경비집행 데이터 정합성 확보**
- 결재 상태(상신/결재중/완료/반려)와 이벤트(환입/변경/취소) 혼재로 집계 기준이 불명확한 문제 해결
- 결재 완료 시점 데이터만을 유효 기준으로 확정하는 원칙 수립 → 운영 중 집계 오류 구조적 차단

**데이터 정합성 검증 배치 설계**
- 단일 결재로 다수 테이블이 변경되는 구조에서 오류 추적을 위한 단계별 금액 검증 배치 구현
- 결재 단계·집행 유형별 검증 쿼리를 배치로 구성 → 오픈 이후 정합성 모니터링 용도로 활용

<br>

## 📋 Other Projects

| 프로젝트 | 기간 | 역할 |
|----------|------|------|
| 카카오뱅크 준법시스템 고도화 지원 | 2025.01 – 2025.04 | 기능 보완 및 테스트 이슈 대응 |
| 다올투자증권 대손충당금 | 2023.08 – 2023.10 | 데이터 검증 및 운영 활용 화면 구축 |
| 농협생명 내부회계 | 2023.06 – 2023.07 | 솔루션 커스터마이징 및 구축 |
| 주택도시보증공사 재무제표 | 2022.12 – 2023.05 | 화면·배치 개발, 결산 안정적 산출 기여 |
| 키움증권 연결 프로젝트 | 2022.06 – 2022.11 | 엑셀 업로드 기반 데이터 사전 검증 고도화 |
| DB저축은행 내부회계 | 2022.04 – 2022.05 | 솔루션 프레임워크 분석 및 배포 지원 |

<br>

## 🔨 Personal Project

### [BonsCore](https://github.com/koobs97/BonsCore) | Spring Boot 3 & Vue 3 프레임워크

> `Spring Boot 3.4` `Spring Security` `JPA` `Oracle` `Redis` `Vue 3` `TypeScript`

실무에서 직접 설계하지 못했거나 더 깊이 이해하고 싶었던 영역들을 직접 구현해본 개인 프로젝트입니다.

- **보안 프레임워크**: XSS 필터, RSA 비대칭키 암호화, JWT + Session 하이브리드 인증, reCAPTCHA
- **공통 모듈**: 전역 응답 래퍼, Global Exception Handler, AOP 기반 로깅·중복요청 방지
- **JPA 심층 활용**: 영속성 컨텍스트, Dirty Checking, Flyway 스키마 버전 관리
- **외부 API 통합**: Kakao Map, Naver DataLab, Google Translate, 기상청 API
- **단위 테스트**: JUnit 5 + Mockito, `@WebMvcTest` / 직접 호출 하이브리드 전략

<br>

## 🏆 Awards & Certifications

| 구분 | 내용 | 연도 |
|------|------|------|
| 자격증 | 정보처리기사 | 2021 |
| 공모전 | 국회도서관 개발 공모전 — 과학기술정보통신부 장관상 🥇 | 2019 |
| 공모전 | 한이음 ICT 개발 공모전 — 한국산업연합회장상 | 2020 |

<br>

## 📬 Contact

- 📱 **Phone**: 010-8702-****
- ✉️ **Email**: koobs97@naver.com
- 💻 **GitHub**: [github.com/koobs97](https://github.com/koobs97)
