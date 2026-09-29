<div align="center">

# Minsu Kang

### Backend & AI Application Developer

AI 기능을 단순히 붙이는 것을 넘어 
서비스에 안정적으로 연결하고 실패 상황까지 처리하는 개발에 관심이 있습니다.

<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
</p>

</div>

---

## Featured Projects

### 📈 TrendIn
**개인화 트렌드 발견을 위한 데이터 처리 파이프라인**  
`Python` · `TF-IDF` · `KeyBERT` · `LLM`

<p align="center">
  <img src="https://raw.githubusercontent.com/minsu42/minsu42/main/images/trendin-explore.png" width="270" alt="TrendIn trend explore"/>
  <img src="https://raw.githubusercontent.com/minsu42/minsu42/main/images/trendin-detail.png" width="270" alt="TrendIn trend detail"/>
  <img src="https://raw.githubusercontent.com/minsu42/minsu42/main/images/trendin-country.png" width="270" alt="TrendIn country trends"/>
</p>

- 크롤링 → 전처리 → 키워드 추출 → 통합 → 지표 산출까지 데이터 파이프라인 전 구간 구현
- 규칙 기반 한국어 처리에서 조사·활용형이 섞이는 문제를 발견하고 형태소 분석 방식으로 전환
- 약어·전개형처럼 근거가 명확한 경우만 자동 병합하고, 애매한 유사도 판단은 검수 대상으로 분리
- 실데이터 리허설을 통해 매핑 결함과 자동 병합 오판정을 줄이고 기준을 보정

---

### 📍 [PinGo](https://github.com/minsu42/pingo)
**지하철 실내 위치추정 기반 XR 내비게이션**  
`Spring Boot` · `FastAPI` · `COLMAP` · `HLOC`

<p align="center">
  <img src="https://raw.githubusercontent.com/minsu42/pingo/master/docs/screenshots/user-flow/04-position-detected.png" width="200" alt="PinGo position detected"/>
  <img src="https://raw.githubusercontent.com/minsu42/pingo/master/docs/screenshots/user-flow/07-ar-navigation.png" width="200" alt="PinGo AR navigation"/>
  <img src="https://raw.githubusercontent.com/minsu42/pingo/master/docs/screenshots/user-flow/08-floor-transition.png" width="200" alt="PinGo floor transition"/>
</p>

- 카메라 이미지를 받아 실내 위치를 추정하는 HLOC/COLMAP 기반 VPS 서버와 서비스 연동 흐름 구현
- 여러 층의 맵을 비교할 때 Query 특징을 한 번만 추출해 각 맵에서 재사용하도록 위치추정 구조 개선
- 단일 프레임의 약한 위치 후보를 여러 프레임에서 누적해 위치를 확정하는 가중 투표 로직 구현
- 카카오 장소·도보 경로 등 외부 API 장애가 전체 안내 흐름을 끊지 않도록 fallback 처리

**🏆 SSAFY 공통 프로젝트 우수상** · [View Repository →](https://github.com/minsu42/pingo)

---

### 🍽 [PlayEat](https://github.com/minsu42/PlayEat)
**AI/RAG를 서비스 로직과 연결한 게임형 건강관리 서비스**  
`Spring Boot` · `Spring AI` · `Qdrant` · `Redis`

<p align="center">
  <img src="https://raw.githubusercontent.com/minsu42/PlayEat/master/images/mainpage.png" width="270" alt="PlayEat main page"/>
  <img src="https://raw.githubusercontent.com/minsu42/PlayEat/master/images/anlayze.png" width="270" alt="PlayEat diet report"/>
  <img src="https://raw.githubusercontent.com/minsu42/PlayEat/master/images/architecture.png" width="270" alt="PlayEat architecture"/>
</p>

- 식단 기록·영양 정보·AI 코칭을 연결하는 백엔드 API와 서비스 로직 구현
- 공식 건강 가이드를 검색해 주간 리포트에 참고자료로 제공하는 RAG 흐름 구성
- Qdrant·외부 AI 제공자 실패가 핵심 기능 전체의 장애로 번지지 않도록 fallback 경로 설계
- LLM의 잘못된 선택이나 불안정한 JSON 응답을 규칙 기반 보정과 파서로 흡수

[View Repository →](https://github.com/minsu42/PlayEat)

---

### ⚡ [Embedded AI](https://github.com/minsu42/EAI)
**Coral Edge TPU 기반 온디바이스 유해조수 탐지·경고 시스템**  
`YOLOv5` · `TFLite` · `Edge TPU` · `C++`

- 유해조수 6개 클래스를 탐지하는 YOLOv5s 모델 학습과 데이터 실험 수행
- 학습 모델을 FP16·INT8 TFLite로 변환하고 EdgeTPU용으로 컴파일해 임베디드 실행 환경에 맞게 경량화
- EdgeTPU 컴파일 결과를 확인하며 대부분의 연산이 TPU에서 실행되도록 모델 변환 과정 검증
- 탐지 결과를 GPIO 부저 경고 로직과 연결하고 텐서 할당 오류 처리 보완

[View Repository →](https://github.com/minsu42/EAI)

---

### 🎮 [TaskArena](https://github.com/minsu42/TaskArena)

**FastAPI 기반 게이미피케이션 태스크 관리 개인 학습 프로젝트**

`FastAPI` · `PostgreSQL` · `React Native` · `Expo` · `OpenAI API`

- 사용자·할 일·점수·랭킹 기능을 구성하며 FastAPI와 PostgreSQL 기반 백엔드 구조를 학습
- React Native/Expo 클라이언트와 REST API를 연결해 모바일·웹 흐름 구현
- OpenAI API를 활용한 할 일 난이도 평가와 피드백 기능을 실험
- Alembic과 Docker Compose를 사용해 스키마 변경과 로컬 개발 환경을 관리

---

## Research

### 🔬 고객의 첫 핵심 질문 품질이 상담 결과에 미치는 영향

**학사 졸업연구**

약 1만 건의 비정형 상담 데이터를 대상으로 연구 변수 정의 → LLM 평가 → 통계 분석까지 직접 수행했습니다.

- 실제 상담에서 인사·서론이 먼저 등장하는 문제를 발견하고, 단순 첫 발화 대신 **'첫 핵심 질문'**을 새로 정의
- 질문 품질 5개·답변 품질 4개 평가 기준과 JSON 출력 스키마를 설계해 LLM 평가 파이프라인 구성
- 대량 호출 과정에서 일부 요청 실패가 전체 분석 중단으로 번지지 않도록 체크포인트와 오류 로그를 적용
- 예상보다 설명력이 낮은 결과를 그대로 받아들이고, 예측 성능보다 회귀분석·SHAP을 통한 관계 해석 중심으로 연구 방향을 정리

`Python` · `LLM Evaluation` · `Prompt Engineering` · `Regression Analysis` · `SHAP`

---

## Core Stack

**Backend**  
`Java` · `Spring Boot` · `FastAPI` · `MySQL` · `PostgreSQL`

**AI / Data**  
`Python` · `RAG` · `Qdrant` · `Computer Vision` · `LLM Application`

**Infra / Embedded**  
`Docker` · `GitHub` · `Raspberry Pi` · `Coral Edge TPU` · `C++`

---

<div align="center">
  <sub>Build AI features that remain useful outside the demo.</sub>
</div>
