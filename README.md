# 📚 hexa-4: 교육/에드테크 AX 마스터클래스

> "교안이 AI로 뚝딱" — 교육/에드테크 중소기업을 위한 AI 자동화 실습 과정

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Reasonofmoon/hexa-4/blob/main/notebooks/M7_EDU_material_lab.ipynb)

---

## 🎯 이 과정은?

**대상**: 학원, 온라인 교육, 교육컨텐츠, edtech 스타트업  
**목표**: 교안 자동 생성·NotebookLM 연동·학습자료 분석 3가지 핵심 자동화  
**시간**: 6시간 (강의 3h + 실습 3h)

---

## 🎯 수준별 활용 가이드

### 🟢 Starter — "5분 안에 교안 초안"
1. `labs/M7-EDU/README.md` 열기
2. 프롬프트 복사 → ChatGPT/뤼튼에 붙여넣기
3. 주제·학습시간·타겟만 수정 후 Enter
4. 교안 즉시 출력 ✅ (코딩 0줄)

### 🔵 Professional — Colab 자동화
```python
# Colab Secret에 저장 (이름: GEMINI_API_KEY)
from google.colab import userdata
api_key = userdata.get('GEMINI_API_KEY')
```
1. Colab 뱃지 클릭 → 노트북 오픈
2. 런타임 → 모두 실행
3. 교육 정보 셀만 수정
4. 교안 + NotebookLM 분석 CSV 자동 다운로드

### 🟣 Enterprise — 멀티 에이전트 파이프라인
- OMC `/team 3:executor`로 분석→교안→Quiz→LMS 연동 자동화
- `AGENTS.md` 기반 교육 보이스 내재화
- `scripts/agents_config_validator.py` 셀프 검증

---

## ⚙️ 3모듈 커리큘럼

| 모듈 | 제목 | Colab | Labs |
|---|---|---|---|
| M1 | AX 진단 & 에듀테크 벤치마킹 | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](notebooks/M1_AX_diagnosis.ipynb) | [labs/M1](labs/M1-diagnosis/) |
| M7-EDU | 교안 자동화 & NotebookLM | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](notebooks/M7_EDU_material_lab.ipynb) | [labs/M7-EDU](labs/M7-EDU/) |
| M9 | LMS 연동 & 자동 평가 시스템 | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](notebooks/M9_lms_auto.ipynb) | [labs/M9](labs/M9-deploy/) |

---

## 📂 프로젝트 구조

```
hexa-4/
├── notebooks/
│   ├── M1_AX_diagnosis.ipynb        ← AX 진단 자동화
│   ├── M7_EDU_material_lab.ipynb     ← 교안 자동화 ★
│   └── M9_lms_auto.ipynb           ← LMS 연동 자동화
├── labs/
│   ├── M1-diagnosis/README.md        ← 진단 프롬프트 모음
│   ├── M7-EDU/README.md             ← 교육 실습 가이드
│   └── M9-deploy/README.md          ← 배포 체크리스트
├── scripts/
│   ├── teaching_material_generator.py ← 교안 생성 (실행 가능)
│   ├── notebooklm_analyzer.py       ← NotebookLM 분석
│   └── agents_config_validator.py   ← AGENTS.md 검증
└── shared/
    └── education_topics_sample.csv   ← 샘플 교육 주제 (30행)
```

---

## 🌐 hexa 시리즈
- [hexa-1](https://github.com/Reasonofmoon/hexa-1): 🏭 제조업
- [hexa-2](https://github.com/Reasonofmoon/hexa-2): 🍽️ 외식/F&B
- [hexa-3](https://github.com/Reasonofmoon/hexa-3): 🛒 소매/유통
- **hexa-4** (현재): 📚 교육/에드테크
- [hexa-5](https://github.com/Reasonofmoon/hexa-5): 🏗️ 건설/부동산
- [hexa-6](https://github.com/Reasonofmoon/hexa-6): 💼 전문서비스/IT

Made with ❤️ by [Reasonofmoon × Antigravity](https://github.com/Reasonofmoon)  
중소기업 AX 전환을 위한 실전 교육