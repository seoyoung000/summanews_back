# SummaNews - Backend (AI News Summarizer) 🚀

**Google Gemini API를 활용한 실시간 뉴스 요약 서버입니다.**  
본 저장소는 'SummaNews' 서비스의 핵심 로직인 뉴스 데이터 추출 및 AI 요약 처리를 담당하는 백엔드 코드를 담고 있습니다.

---

## 🛠 주요 기능
- **AI 뉴스 요약**: Google Gemini API(Gemini Pro)를 연동하여 긴 뉴스 기사를 3문장 이내의 핵심 요약문으로 변환.
- **데이터 처리**: 뉴스 기사 본문 텍스트의 전처리 및 요약 모델 최적화 프롬프트 관리.
- **서버 환경**: Jupyter Notebook(ipynb) 환경을 통한 API 테스트 및 데이터 응답 구조 설계.

## ⚙️ 기술 스택
- **Language**: Python 3.x
- **AI Model**: Google Gemini API (Generative AI)
- **Environment**: Google Colab / Jupyter Notebook
- **Library**: `google-generativeai`, `pandas`, `json`

## 📊 프로젝트 결과물 (발표 자료)
- **최종 발표 자료**: [졸업작품 최종발표_수정.pdf](./졸업작품%20최종발표_수정.pdf)
  - 서비스 기획 배경, 시스템 아키텍처, 기대 효과 등에 대한 상세 내용이 포함되어 있습니다.

## 🚀 실행 및 구성
1. `summanews_server(Gemini_API).ipynb` 파일을 실행합니다.
2. 개인의 `GEMINI_API_KEY`를 설정 파일 또는 환경 변수에 입력합니다.
3. 입력된 뉴스 데이터를 API를 통해 요약된 JSON 형태로 반환합니다.

---

## 🔗 관련 프로젝트
- **Frontend**: [SummaNews-Frontend](https://github.com/seoyoung000/summanews-frontend) (React Native 기반 모바일 앱)