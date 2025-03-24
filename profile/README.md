# 🍺BrauHaus

<img width="100%" alt="mainw" src="https://github.com/user-attachments/assets/39799ff4-d68a-4190-b846-46f1dc7daa76" />
<br/>

<br/>
프로젝트 기간 25.02.03 ~ 25.03.17 <br/>


---
👍 [meeting](https://github.com/QualityCore/QualityCore-backend/discussions/categories/meeting?discussions_q=) | 
👍 [Front-PR](https://github.com/QualityCore/QualityCore-frontend/pulls?q=is%3Apr+is%3Aclosed) | 
👍 [Back-PR](https://github.com/QualityCore/QualityCore-backend/pulls?q=is%3Apr+is%3Aclosed) | 
👍 [Front-Issues](https://github.com/QualityCore/QualityCore-frontend/issues?q=is%3Aissue%20state%3Aclosed) | 
👍 [Back-Issues](https://github.com/QualityCore/QualityCore-backend/pulls?q=is%3Apr+is%3Aclosed) | 
<br/>

---

## 🧭 빠른 이동
- [프로젝트 소개](#프로젝트-소개)
- [프로젝트 일정](#프로젝트-일정)
- [아키텍쳐](#아키텍쳐)
- [기술 스택](#기술-스택)
- [기능 설명](#기능-설명)
- [논리 & 물리 데이터 모델링](#논리--물리-데이터-모델링)
---

<a name = "프로젝트-소개"></a>
## 📌 프로젝트 소개

맥주 제조 공정의 생산부터 출하까지 전반적인 과정을 **직관적으로 관리할 수 있도록 설계된 ERP 프로젝트**입니다.<br/>
실제 양조 라인의 작업 흐름을 반영하여 **생산 계획 수립, 공정 제어, 실적 분석까지 통합 관리**할 수 있도록 구현하였습니다.<br/>
단순한 정보 나열이 아닌, **현장 중심의 실질적인 생산 관리 UX 구현**에 초점을 맞추었습니다. <br/> 
작업 지시, 공정 실행, 스케줄 확인 등 주요 업무는 사용자 친화적인 모달, 캘린더, 대시보드 등을 통해 처리됩니다.<br/>
<br/>
 
### 🍺 BrauHaus 주요 기능
 
#### ✅ 1. 생산 계획 수립 및 실행 흐름 지원
 - 월별/일별 생산계획을 등록하고 작업지시서 자동 발행  
 - 공정별 작업 실행 화면에서 **각 단계별 진행 상태 시각화**  
 - 직원별 담당 공정 확인 및 **스케줄 자동 생성 기능** 포함  
 - 자재 소요량 계산 기반의 구매 요청 연동 (기초 로직 구현)
 
 #### ✅ 2. 공정 흐름 및 라우팅 관리
 - 당화 → 여과 → 끓임 → 냉각 → 발효 → 숙성 등 **맥주 양조 흐름 시스템화**
 - 공정별 작업 상태를 **실시간 카드 뷰 + 타이머**로 확인 가능  
 - 제품별 라우팅 자동 구성, 워크플로우 오류 감지로 **불량률 예방 시도**
 
 #### ✅ 3. 생산 실적 모니터링 및 분석
 - 월별 계획 대비 실적, 공정별 효율성 등 **대시보드 제공**  
 - KPI 기반 생산성/불량률 시각화 및 히트맵 UI로 이상 흐름 인지  
 - **공정별 랭킹**, 실시간 상태 표시 등으로 관리자 대응 효율 향상
 
 
 💡 *본 프로젝트는 실제 ERP 구조를 바탕으로 프론트/백엔드 연동과 UX 시뮬레이션을 중심으로 구현되었으며,  
 일부 보안 및 인증 기능은 개발 범위 외로 처리되었습니다.*
 
 - [📒 팀 노션](https://www.notion.so/ohgiraffers/QualityCore-7920de328e0346fc91ac1beb96191344)
 - [🏳️‍🌈 Figma](https://www.figma.com/design/KaKLszFW3IRpA7HM89VoiI/Qulity_Core?node-id=0-1&p=f&t=5U3P5uWp6YptJbit-0)

 
 ---

 
 <a name = "프로젝트-일정"></a>
 ## 📌 프로젝트 일정
<img width="100%" alt="TimeLine" src="https://github.com/user-attachments/assets/7da436a3-9163-476d-b333-8682987ff97e" />

---


<a name ="아키텍쳐"></a>
## 📌 아키텍쳐

<p>조금만 더 공부 좀해볼께요</p>

---




<a name = "기술-스택"></a>
## 📌 기술 스택


### 🧠 Backend
| 구분 | 사용 기술 |
|------|-----------|
| **프레임워크 & 언어** | Java 17, Spring Boot |
| **ORM & DB** | Spring Data JPA, MyBatis, Hibernate, OracleDB |
| **쿼리** | QueryDSL |
| **템플릿 엔진** | Thymeleaf |
| **보안 & 인증** | JWT 로그인 기능 구현 예정 (팀원 이탈로 미완성) |
| **API 문서화** | SpringDoc OpenAPI (Swagger) |
| **모델 매핑** | ModelMapper |
| **웹소켓** | Spring Boot WebSocket (STOMP) |
| **이메일 전송** | JavaMailSender (SMTP, Gmail 연동) |
| **PDF/문서 처리** | Apache POI (Excel 처리) |
| **파일 업로드** | Cloudinary (cloudinary-core, cloudinary-http44) |
| **입력 검증** | Spring Validation (JSR-380) |
| **로그 & AOP** | Lombok (@Slf4j), Spring AOP |
| **배포 환경** | 로컬 개발 환경 (Oracle DB 기준), Railway 배포 고려 중|
| **테스트** | JUnit, MyBatis Test |
| **기타 도구** | DevTools, ojdbc8 / ojdbc11 드라이버 |

<br/>
<br/>

## 🎨 Frontend 기술 스택

| 구분 | 기술 |
|------|------|
| **프레임워크** | React |
| **기본 기술** | HTML5, CSS3, JavaScript |
| **라우팅** | React Router DOM |
| **상태 관리** | useState, useEffect, useMemo, useCallback |
| **HTTP 통신** | fetch API, axios |
| **UI 구성** | MUI, Lucide-React, Chart.js |
| **모달 처리** | react-modal |
| **애니메이션** | Lottie-React, JS-Confetti |
| **이미지 처리** | Lazy Loading, Canvas API (라벨 그리기) |
| **파일 업로드** | Blob 변환 후 Multipart 전송 |
| **마크다운 렌더링** | marked |
| **사용자 인증** | Context API (useAuth) |
| **스타일링** | CSS Modules, Flexbox 기반 레이아웃 |
| **반응형** | Media Query (모바일 대응) |
| **마이크로 UX** | Gradient, Hover, Shadow, Transition 효과 |
| **기타** | 단계별 플로우 구성, 커스텀 캘린더, 공정 카드 뷰 |

<br/>
<br/>


## ☁️ 파일 저장 & 데이터 백업

| 구분 | 기술 |
|------|------|
| **DB 백업 & 복제** | Oracle XE (로컬 환경, 별도 복제 구성 없음) |

“현재는 Oracle XE 기반 로컬 저장소에서 테스트 진행했으며, 추후 클라우드 파일 저장소 및 DB 이중화 구성을 고려 중입니다.”
<br/>
<br/>

---


<a name="기능-설명"></a>
## 📌 기능 설명

### 로그인

### 생산계획

### 생산지시

### 생산공정 관리

### Routing 관리

...

<br/>
<br/>

---

<a name="논리--물리-데이터-모델링"></a>
## 📌 논리 데이터 모델링 ( 총 32개 테이블 )
<img width="100%" alt="생산 ERP 모델링" src="https://github.com/user-attachments/assets/0e366ad1-b38f-4663-a446-1cd0cfef48fa" />

<br/>
<br/>

---

