# Minsu Kang

백엔드 시스템을 기반으로 AI 기능을 서비스에 안정적으로 연결하는 개발자를 지향합니다.

- 숭실대학교 AI융합학부 졸업 (2022.03 ~ 2026.02)
- SSAFY 15기 Backend Track 교육 중 (2026.01 ~ )
- 관심 분야: Spring Boot, AI 서비스 연동, 데이터 기반 기능 설계, 서비스 운영 자동화

---

## Tech Stack

**Backend**
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/MyBatis-DB2A2A?style=flat-square"/>
  <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
</p>

**AI / Data**
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat-square"/>
  <img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square"/>
  <img src="https://img.shields.io/badge/RAG-333333?style=flat-square"/>
  <img src="https://img.shields.io/badge/YOLO-111F68?style=flat-square"/>
  <img src="https://img.shields.io/badge/TensorFlow%20Lite-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
</p>

**Frontend / Cross-stack**
<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/React%20Native-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white"/>
  <img src="https://img.shields.io/badge/Zustand-433E38?style=flat-square"/>
</p>

**Infra / Tools**
<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=white"/>
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white"/>
</p>

**Embedded / Vision**
<p>
  <img src="https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Coral%20Edge%20TPU-4285F4?style=flat-square"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/wiringPi-A22846?style=flat-square"/>
</p>

---

## Featured Projects

### [냠냠코치 / PlayEat](https://github.com/minsu42/PlayEat)

> 식단 기록을 AI 분석, 캐릭터 성장, 길드 보스전, 상점 보상으로 연결한 게임형 건강 관리 서비스

<p>
  <img src="https://raw.githubusercontent.com/minsu42/PlayEat/master/images/mainpage.png" width="360"/>
  <img src="https://raw.githubusercontent.com/minsu42/PlayEat/master/images/bosspage.png" width="360"/>
</p>

**Tech**
Spring Boot 3.3.5, MyBatis, MySQL, Redis, Spring AI, Qdrant

**Role**
2인 팀 프로젝트에서 백엔드 중심 개발과 일부 프론트엔드 API 연동을 담당했습니다.

**Key Contributions**
- 이메일 로그인, Google OAuth 로그인, JWT 인증 플로우 구현
- 온보딩 기반 건강 정보 입력과 초기 캐릭터 선택 플로우 설계
- 음식 검색, 끼니별 식단 기록 CRUD, 영양소 자동 계산 로직 구현
- 일일 영양 합계 갱신 로직을 설계해 식단 기록과 건강 상태 분석을 연결
- AI 리포트 결과를 `NORMAL`, `HUNGRY`, `CHUBBY`, `MUSCLE` 캐릭터 상태 전이 로직에 연동
- 식품영양성분 데이터 기반 RAG 파이프라인 구축
- Spring AI + Qdrant를 활용해 일간/주간 AI 코칭 리포트 생성
- `@TransactionalEventListener(phase = AFTER_COMMIT)`를 활용해 식단 기록 트랜잭션 성공 이후에만 경험치와 캐릭터 상태 변화가 반영되도록 설계

**Technical Focus**
- 인증/인가 구조
- 식단 기록 기반 비즈니스 로직
- AI 리포트와 서비스 상태 변화 연동
- 이벤트 기반 캐릭터 성장 처리
- RAG 기반 개인화 코칭

---

### [유해 조수 탐지 프로젝트 / EAI](https://github.com/minsu42/EAI)

> 라즈베리파이와 Coral Edge TPU를 활용한 온디바이스 실시간 유해 조수 탐지·퇴치 시스템

이 레포는 팀 프로젝트를 진행한 팀원(KimGeonWoo-p)의 저장소이며, 본인은 팀원으로 참여해 아래 항목을 담당했습니다.

**Tech**
Python, YOLOv5, YOLOv11, TensorFlow Lite, Edge TPU, OpenCV, C++, Raspberry Pi

**Role**
임베디드 프로그래밍 수업 팀 프로젝트에서 모델 학습, 경량화, 온디바이스 추론 로직을 담당했습니다.

**Key Contributions**
- YOLOv5 / YOLOv11 기반 커스텀 데이터셋 학습 및 라벨링 노트북 작성
- 학습 모델을 FP16 / INT8로 양자화하고 Edge TPU 컴파일까지 이어지는 변환 파이프라인 구축
- OpenCV와 TensorFlow Lite Edge TPU delegate를 활용해 라즈베리파이 카메라(`/dev/video0`) 실시간 프레임 추론 구현
- C++ 기반 추론 실행 로직 작성
- IoU 기반 NMS(Non-Max Suppression)를 직접 구현해 중복 바운딩 박스 제거
- 탐지 결과에 따라 wiringPi 기반 GPIO 부저를 제어하는 `warning_on()` / `warning_off()` 모듈 구현

**Technical Focus**
- 온디바이스 AI 추론
- 모델 경량화 및 Edge TPU 최적화
- 실시간 객체 탐지
- C++ 기반 하드웨어 제어
- 임베디드 환경에서의 AI 모델 실행

---

### [TaskArena](https://github.com/minsu42/TaskArena)

> 할 일을 완료하고 친구와 배틀하며 랭킹을 올리는 게이미피케이션 태스크 관리 앱

개인 프로젝트로 기획부터 백엔드/프론트엔드 구현, 배포까지 전 과정을 혼자 진행했습니다.

**Tech**
FastAPI, SQLAlchemy 2.0, PostgreSQL, React Native, Expo, TypeScript, Zustand, OpenAI API

**Role**
개인 프로젝트로 백엔드, 프론트엔드, AI 연동, 배포 환경을 전체 설계하고 구현했습니다.

**Key Contributions**
- JWT 인증 기반 사용자 로그인 구조 구현
- SQLAlchemy 2.0과 Alembic을 활용한 데이터 모델링 및 마이그레이션 관리
- GPT-3.5 기반 할 일 난이도 평가 기능 구현
- 완료 내역 기반 맞춤형 AI 피드백 생성 기능 구현
- 일일 점수 계산 로직 설계
  `일일 점수 = (완료율 × 0.5 + 난이도 가중 완료율 × 0.5) × 100`
- 친구와 1:1 배틀을 진행하고 K=32 기준 ELO 레이팅을 반영하는 랭킹 시스템 구현
- Zustand를 활용해 토큰과 사용자 상태를 관리하는 프론트엔드 구조 설계
- Render, Vercel, Docker Compose를 활용해 배포 및 로컬 실행 환경 구성

**Technical Focus**
- 개인 프로젝트 전체 설계
- 인증과 사용자 상태 관리
- AI 기반 자동 평가
- 게임형 점수/랭킹 시스템
- 백엔드·프론트엔드 통합 구현

---

## Problem Solving Highlights

### Transactional Event Handling

PlayEat에서는 식단 기록이 성공적으로 저장된 이후에만 캐릭터 경험치와 상태 변화가 반영되어야 했습니다.
이를 위해 `@TransactionalEventListener(phase = AFTER_COMMIT)`를 사용해 트랜잭션 커밋 이후 성장 이벤트가 실행되도록 설계했습니다.

이 구조를 통해 식단 저장에 실패했는데도 캐릭터 상태가 변경되는 데이터 불일치 가능성을 줄였습니다.

---

### RAG-based AI Report

PlayEat의 AI 리포트는 단순한 일반 답변이 아니라, 식품영양성분 데이터를 기반으로 생성되도록 구성했습니다.
Spring AI와 Qdrant를 활용해 관련 영양 정보를 검색하고, 검색 결과를 바탕으로 일간/주간 식단 코칭 리포트를 생성했습니다.

이 과정에서 사용자 식단 기록과 외부 영양성분 데이터를 연결해 개인화된 피드백을 제공할 수 있도록 했습니다.

---

### On-device Vision Inference

EAI 프로젝트에서는 서버 의존도를 낮추기 위해 라즈베리파이와 Coral Edge TPU 기반 온디바이스 추론 구조를 구성했습니다.
학습된 YOLO 모델을 양자화하고 Edge TPU에서 실행 가능한 형태로 변환한 뒤, OpenCV 카메라 입력과 C++ 추론 로직을 연결했습니다.

이를 통해 실시간 카메라 입력에서 유해 조수를 탐지하고, GPIO 부저 제어까지 이어지는 흐름을 구현했습니다.

---

## Currently Focusing On

- Spring Boot 기반 백엔드 설계 역량 강화
- 인증/인가, 트랜잭션, 데이터 모델링 학습
- AI 기능을 실제 서비스 흐름에 안정적으로 연결하는 구조 설계
- 테스트 코드와 배포 자동화를 통한 서비스 신뢰성 개선

---

## Contact

- Email: kangms2023@naver.com
- GitHub: https://github.com/minsu42
- Velog: https://velog.io/@kangms2023
