<div align="center">

# 📚 hexa-4: 교육 AX 마스터클래스

### *AI로 교육 현장을 혁신하는 12주 실전 과정*

**교안자동화부터 학습분석까지 — 학습 데이터로 직접 검증하는 AX 커리큘럼**

[![Version](https://img.shields.io/badge/version-1.0.0-6366f1?style=for-the-badge)](https://github.com/Reasonofmoon/hexa-4)
[![Colab](https://img.shields.io/badge/Google_Colab-12개_노트북-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://github.com/Reasonofmoon/hexa-4/tree/main/notebooks)
[![Sector](https://img.shields.io/badge/Sector-Education-2563eb?style=for-the-badge&logo=graduation-cap&logoColor=white)](https://github.com/Reasonofmoon/hexa-4)
[![License](https://img.shields.io/badge/License-MIT-a78bfa?style=for-the-badge)](LICENSE)
[![Scripts](https://img.shields.io/badge/CLI_Scripts-8개-22d3ee?style=for-the-badge&logo=python)](scripts/)

> **"교육 현장에서 AI 도구를 사용할 수 있는 교사는 전체의 4% 미만이다."**  
> hexa-4는 코딩 경험이 없는 강사·교육 관리자도 Colab 노트북으로  
> 바로 실전 결과를 내도록 설계된 **12주 실무 중심 AX 커리큘럼**입니다.

[📗 커리큘럼 시작](notebooks/) · [🔧 스크립트 도구](scripts/) · [📂 실습 데이터](shared/) · [🐛 이슈](../../issues)

</div>

---

## 🧠 Philosophy — "왜 교육 AX인가"

기존 교육 AI 교육의 문제: **학습 데이터가 없이 이론만 있다**.

| 기준 | 기존 AI 교육 | hexa-4 AX 커리큘럼 |
|------|-------------|-------------------|
| 데이터 | 가상의 학습 데이터 | **실제 수업 CSV** (성적, 출결, 평가) |
| 결과물 | 모델 정확도 숫자 | **개인화 교안 + 학부모 알림 + 챗봇** |
| 난이도 | Python 필수 | **Colab 실행만으로 완성** |
| 기간 | 3개월+ 이론 | **Week 1부터 실전 결과** |
| 연결성 | 개별 실습 | **W1→W12 파이프라인으로 연결** |

```mermaid
graph LR
    A[📋 W1-2 진단&교안] --> B[📝 W3-4 레벨테스트]
    B --> C[📊 W5-6 성적분석]
    C --> D[📨 W7-8 챗봇&알림]
    D --> E[🔮 W9-10 수업품질분석]
    E --> F[🎛️ W11-12 통합대시보드]
    
    style A fill:#6366f1,color:#fff
    style F fill:#22d3ee,color:#fff
```

---

## ⚙️ 시스템 레이어

### Layer 1 · Foundation (W1~W4) — AI 기초 도구화
> **Wow**: 10개 강의 주제를 AI가 **5초 안에** 교안으로 자동 생성

| 주차 | 노트북 | 핵심 도구 |
|------|--------|-----------|
| W1 | M1_AX_diagnosis.ipynb | Gemini API, 자가진단 |
| W2 | W02_teaching_automation.ipynb | 교안 자동 생성, 난이도 조절 |
| W3 | W03_level_test.ipynb | 레벨 테스트, 맞춤형 문제 |
| W4 | W04_feedback_automation.ipynb | 자동 피드백, 개별 코칭 |

### Layer 2 · Analytics (W5~W8) — 데이터 기반 의사결정
> **Wow**: 성적·출결·학습 패턴을 **클릭 한 번**에 학습자 차트로 변환

| 주차 | 노트북 | 핵심 도구 |
|------|--------|-----------|
| W5 | W05_grade_analysis.ipynb | pandas, matplotlib, 성적 트렌드 |
| W6 | W06_learning_progress.ipynb | 학습 진도, 개인화 경로 |
| W7 | W07_chatbot.ipynb | 교육 챗봇, Q&A 자동화 |
| W8 | W08_parent_notification.ipynb | 학부모 알림, 성적 공유 |

### Layer 3 · Intelligence (W9~W12) — 자동화 운영 시스템
> **Wow**: 학습 부족 시 **자동 보충자료 → 학부모 알림 → 맞춤 과제** 파이프라인

| 주차 | 노트북 | 핵심 도구 |
|------|--------|-----------|
| W9 | W09_class_quality_analysis.ipynb | 수업 품질 분석, 개선점 도출 |
| W10 | W10_calendar_sync.ipynb | 학습 캘린더, 스케줄 자동화 |
| W11 | W11_education_dashboard.ipynb | 종합 교육 대시보드 |
| W12 | W12_integrated_operation.ipynb | 통합 운영 시스템 발표 |

---

## 🎯 수준별 활용 가이드

### 🟢 Starter — "5분 안에 첫 결과"
1. [W2 노트북](https://colab.research.google.com/github.com/Reasonofmoon/hexa-4/blob/main/notebooks/W02_teaching_automation.ipynb) 클릭 → Colab에서 열기
2. `EDUCATION_INFO`에 과목명·학습시간만 입력 (`✏️` 표시 찾기)
3. `Shift+Enter`로 위에서 아래로 실행
4. 맞춤형 교안 + 레벨 테스트 자동 다운로드

> ⚠️ API 키 발급: [Google AI Studio](https://aistudio.google.com/apikey) → GEMINI_API_KEY

### 🔵 Professional — "내 학습 데이터로 실전 분석"
1. `shared/education_topics_sample.csv` 구조 확인
2. 내 학습 데이터를 같은 형식으로 준비
3. W5~W6 노트북에서 CSV 업로드 → 성적·학습 패턴 자동 분석
4. W8 노트북에서 학부모 알림 연결 → 자동 성적 공유

```bash
# CLI 스크립트 직접 사용
python scripts/teaching_material_generator.py --input shared/education_topics_sample.csv
python scripts/grade_analyzer.py --input data.csv --output results.csv
python scripts/parent_notifier.py --input data.csv --webhook [WEBHOOK_URL]
```

### 🟣 Enterprise — "팀 표준화 & 파이프라인"
1. `scripts/M9_demo_runner.py` 실행 → 전체 파이프라인 원클릭 시연
2. GitHub Actions로 매일 자동 학습 진도 스케줄링
3. W11~W12를 내부 대시보드로 배포 (Flask/Streamlit)
4. hexa-1, hexa-5와 연계해서 업종 간 벤치마킹

---

## 📂 디렉토리 구조

```
hexa-4/
├── notebooks/          ← 12주 Colab 노트북 (W01~W12)
│   ├── W02_teaching_automation.ipynb     # 교안 자동 생성기
│   ├── W03_level_test.ipynb             # 레벨 테스트
│   ├── W04_feedback_automation.ipynb     # 자동 피드백
│   ├── W05_grade_analysis.ipynb          # 성적 분석
│   ├── W06_learning_progress.ipynb       # 학습 진도 분석
│   ├── W07_chatbot.ipynb                # 교육 챗봇
│   ├── W08_parent_notification.ipynb      # 학부모 알림
│   └── W09_class_quality_analysis.ipynb   # 수업 품질 분석
├── scripts/            ← CLI 실행 가능 Python 스크립트
│   ├── teaching_material_generator.py     # 교안 생성기
│   ├── level_test_generator.py          # 레벨 테스트 생성
│   ├── grade_analyzer.py               # 성적 분석기
│   ├── learning_progress_tracker.py     # 학습 진도 추적
│   ├── education_chatbot.py            # 교육 챗봇
│   ├── parent_notifier.py              # 학부모 알림
│   ├── class_quality_analyzer.py       # 수업 품질 분석
│   └── M9_demo_runner.py              # 원클릭 데모 런처
├── shared/             ← 실습 데이터
│   ├── education_topics_sample.csv      # 교육 주제 샘플
│   └── student_performance_sample.csv  # 학생 성적 샘플
└── labs/               ← 실습 가이드 (M2~M7)
    ├── M2-teaching/README.md
    ├── M3-level/README.md
    ├── M4-feedback/README.md
    └── M7-education/README.md
```

---

## 🔧 확장 가이드

| 우선순위 | 커스터마이징 | 난이도 | 영향 범위 |
|----------|--------------|--------|-----------|
| **1st** | `EDUCATION_INFO` 딕셔너리 수정 | ⭐ | 과목명·학습시간·난이도 |
| **2nd** | 샘플 CSV를 실제 데이터로 교체 | ⭐⭐ | 분석 결과 전체 |
| **3rd** | 학부모 알림 Webhook 연결 | ⭐⭐ | 실시간 공유 |
| **4th** | LMS API 인증 설정 | ⭐⭐⭐ | 시스템 연동 |
| **5th** | W11~W12 대시보드 서버 배포 | ⭐⭐⭐ | 팀 공유 시스템 |

---

## 🚀 빠른 시작

```bash
# 1. 레포 클론
git clone https://github.com/Reasonofmoon/hexa-4.git
cd hexa-4

# 2. 환경 설정 (로컬 실행 시)
pip install google-generativeai pandas matplotlib gspread requests

# 3. 데모 실행
python scripts/M9_demo_runner.py

# 4. 교안 생성 바로 실행
python scripts/teaching_material_generator.py --input shared/education_topics_sample.csv
```

또는 **Colab에서 바로 실행** (설치 불필요):  
[![W2 열기](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github.com/Reasonofmoon/hexa-4/blob/main/notebooks/W02_teaching_automation.ipynb)
[![W6 열기](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github.com/Reasonofmoon/hexa-4/blob/main/notebooks/W06_learning_progress.ipynb)
[![W9 열기](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github.com/Reasonofmoon/hexa-4/blob/main/notebooks/W09_class_quality_analysis.ipynb)

---

## 🔗 전체 AX 시리즈

| 레포 | 섹터 | 핵심 모듈 |
|------|------|-----------|
| [hexa-1](https://github.com/Reasonofmoon/hexa-1) | 🏭 제조업 | OEE, 불량분류, 예지보전 |
| [hexa-2](https://github.com/Reasonofmoon/hexa-2) | 🍽️ F&B | 리뷰분석, 메뉴카피, 재고예측 |
| [hexa-3](https://github.com/Reasonofmoon/hexa-3) | 🛒 소매/유통 | 상품카피, CRM, SEO |
| **hexa-4** (현재) | 📚 교육 | 교안자동화, 성적분석, 챗봇 |
| [hexa-5](https://github.com/Reasonofmoon/hexa-5) | 🏗️ 건설 | 계약서분석, 공정관리 |
| [hexa-6](https://github.com/Reasonofmoon/hexa-6) | 💼 IT/서비스 | 제안서, 코드리뷰, KPI |

---

## 🌐 다국어 지원

| 항목 | 현황 |
|------|------|
| 노트북 UI | 한국어 |
| 스크립트 출력 | 한국어 (컬럼 자동감지: 한/영) |
| 샘플 데이터 | 한국어 컬럼명 |
| README | 한국어 / English (예정) |

---

*AX Consulting Curriculum © 2026 | Powered by Google Gemini*