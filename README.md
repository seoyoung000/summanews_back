# SummaNews - Backend (AI News Summarizer) 🚀

**Google Gemini API와 Flask를 활용한 실시간 뉴스 수집 및 요약 서버입니다.**  
본 저장소는 'SummaNews' 서비스의 핵심 로직인 뉴스 크롤링, AI 요약 처리, 그리고 모바일 앱과의 통신을 위한 API 서버 코드를 담고 있습니다.

---

## 🛠 주요 기능
- **AI 뉴스 요약**: `gemini-2.5-flash` 모델을 사용하여 뉴스 기사를 핵심 정보 위주(300자 이내)로 자동 요약.
- **뉴스 크롤링**: `newspaper3k` 및 `trafilatura`를 활용하여 다양한 뉴스 매체에서 본문 텍스트 추출.
- **유사도 분석**: `scikit-learn`의 TF-IDF 및 코사인 유사도를 활용하여 중복되거나 유사한 기사를 필터링.
- **REST API 서버**: Flask를 통해 프론트엔드(React Native)와 실시간 데이터 송수신.
- **터널링 서비스**: `pyngrok`을 활용하여 로컬/Colab 환경의 서버를 외부 서버로 공개.

## ⚙️ 기술 스택
- **Language**: Python 3.x
- **AI Model**: Google Gemini API (`gemini-2.5-flash`)
- **Backend Framework**: Flask, Flask-CORS
- **Crawling & Scraping**: `newspaper3k`, `trafilatura`, `BeautifulSoup4`
- **Machine Learning/NLP**: `scikit-learn` (TfidfVectorizer, Cosine Similarity)
- **Networking**: `pyngrok`, `requests`, `nest_asyncio`

## 📊 프로젝트 결과물 (발표 자료)
- **최종 발표 자료**: [졸업작품 최종발표_수정.pdf](./졸업작품%20최종발표_수정.pdf)
  - 서비스 기획 배경, 시스템 아키텍처, 기대 효과 등에 대한 상세 내용이 포함되어 있습니다.

## ⚠️ 보안 안내
- 프로젝트 코드 내의 API Key(Gemini, Naver, Ngrok)는 환경 변수(`os.environ`)를 통해 관리하는 것이 권장됩니다.
- 현재 코드에 포함된 키 값은 테스트용이며, 실제 배포 시 반드시 별도의 보안 관리가 필요합니다.

## 🚀 실행 및 구성
1. 필요한 패키지를 설치합니다: `pip install flask flask-cors requests beautifulsoup4 pyngrok newspaper3k scikit-learn trafilatura`
2. `summanews_server(Gemini_API).ipynb` 파일을 실행합니다.
3. Ngrok을 통해 생성된 Public URL을 프론트엔드 앱의 API 주소로 설정합니다.

---

## 🔗 관련 프로젝트
- **Frontend**: [SummaNews-Frontend](https://github.com/seoyoung000/summanews-frontend) (React Native 기반 모바일 앱)
