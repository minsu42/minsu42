<h1 align="center">Hi 👋, I'm Minsu Kang</h1>

---

### 🙋 About Me

- 🎓 숭실대학교 AI융합학부 졸업 ( 22.03 ~ 26.02 )
- 💻 SSAFY 15기 백엔드 트랙 교육 중 ( 26.01 ~ )

---

### 🛠 Tech Stack

**Backend**
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/MyBatis-DB2A2A?style=flat-square"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
</p>

**AI / Data**
<p>
  <img src="https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat-square"/>
  <img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square"/>
  <img src="https://img.shields.io/badge/RAG-333333?style=flat-square"/>
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white"/>
</p>

**Cross-stack (TaskArena)**
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/React%20Native-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
</p>

**Embedded / Vision (EAI)**
<p>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow%20Lite-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Coral%20Edge%20TPU-4285F4?style=flat-square"/>
  <img src="https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white"/>
</p>

**Tools**
<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white"/>
</p>

---

### 📌 Featured Projects

#### 🍚 [냠냠코치 (PlayEat)](https://github.com/minsu42/PlayEat)
식단 기록을 AI 분석·캐릭터 성장·길드 보스전·상점 보상으로 연결하는 게임형 건강 관리 서비스 — Spring Boot 3.3.5 / MyBatis / MySQL / Redis / Spring AI + Qdrant (2인 팀 프로젝트, Backend 중심 + 일부 Frontend)

- 이메일/Google OAuth 로그인 + JWT 인증, 온보딩 기반 건강 정보 입력과 초기 캐릭터 선택 플로우 구현
- 음식 검색·끼니별 식단 기록 CRUD와 영양소 자동 계산·일일 영양 합계 갱신 로직 설계
- NORMAL/HUNGRY/CHUBBY/MUSCLE 캐릭터 상태 전이 로직으로 AI 리포트 결과를 캐릭터 변화에 실시간 연동
- 식품영양성분 데이터 기반 RAG 파이프라인 구축 (top-K=5, 유사도 임계값 0.5)으로 일간/주간 AI 코칭 리포트 생성
- 이벤트 기반 캐릭터 성장·스트릭 처리: @TransactionalEventListener(phase = AFTER_COMMIT)로 트랜잭션 성공 후에만 경험치·상태 변화가 반영되도록 설계


#### 🐦 [유해 조수 탐지 프로젝트 (EAI)](https://github.com/KimGeonWoo-p/EAI)
라즈베리파이 + Coral Edge TPU 기반 온디바이스 실시간 유해 조수 탐지·퇴치 시스템 — 임베디드 프로그래밍 수업 팀 프로젝트 (담당: 모델 학습·경량화 및 온디바이스 추론 로직)

- YOLOv5 / YOLOv11 커스텀 데이터셋 학습 및 라벨링 노트북 작성, 모델을 FP16 / INT8로 양자화 후 Edge TPU 컴파일까지 변환 파이프라인 구축
- OpenCV + TensorFlow Lite(Edge TPU delegate)로 라즈베리파이 카메라(`/dev/video0`) 실시간 프레임을 받아 C++로 추론 실행
- IoU 기반 NMS(Non-Max Suppression)를 직접 구현해 중복 바운딩 박스를 제거하고 탐지 신뢰도를 필터링
- wiringPi로 GPIO 부저(buzzer)를 제어하는 `warning_on()/warning_off()` 모듈을 만들어, 유해 조수 감지 시 실제 하드웨어 경고 신호로 연결

#### ⚔️ [TaskArena](https://github.com/minsu42/TaskArena)
할 일을 완료하고 친구와 배틀하며 랭킹을 올리는 게이미피케이션 태스크 앱 — FastAPI / SQLAlchemy 2.0 / PostgreSQL + React Native(Expo) / TypeScript (개인 프로젝트, 백엔드·프론트엔드 전체 설계/구현)

- GPT-3.5 기반 AI 난이도 평가: 할 일의 제목·설명을 분석해 난이도(상/중/하) 자동 부여, 완료 내역 기반 맞춤형 AI 피드백 생성
- 일일 점수 = `(완료율 × 0.5 + 난이도 가중 완료율 × 0.5) × 100` 공식으로 친구와 1:1 배틀, K=32 표준 공식의 ELO 레이팅 반영
- JWT 인증(python-jose) + Alembic 마이그레이션 기반 백엔드, Zustand로 토큰·유저 상태를 관리하는 프론트엔드
- Render.com(백엔드+PostgreSQL) / Vercel(프론트 웹) / Docker Compose(로컬)로 실제 배포까지 완료

---

### 📫 Contact

- Email: kangms2023@naver.com
- Velog: https://velog.io/@kangms2023
