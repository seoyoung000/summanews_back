SummaNews Back-end

---

## 🛠 주요 기능
- **AI 뉴스 요약**: `gemini-2.5-flash` 모델을 사용하여 뉴스 기사를 핵심 정보 위주(300자 이내)로 자동 요약.
- **뉴스 크롤링**: `newspaper3k` 및 `trafilatura`를 활용하여 다양한 뉴스 매체에서 본문 텍스트 추출.
- **유사도 분석**: `scikit-learn`의 TF-IDF 및 코사인 유사도를 활용하여 중복되거나 유사한 기사를 필터링.
- **REST API 서버**: Flask를 통해 프론트엔드(React Native)와 실시간 데이터 송수신.
- **터널링 서비스**: `pyngrok`을 활용하여 로컬/Colab 환경의 서버를 외부 서버로 공개.

## ⚙️ 기술 스택
- **Language**: Python 3.x
- **AI Model**: Google Gemini API
- **Backend Framework**: Flask, Flask-CORS
- **Crawling & Scraping**: `newspaper3k`, `trafilatura`, `BeautifulSoup4`
- **Machine Learning/NLP**: `scikit-learn` (TfidfVectorizer, Cosine Similarity)
- **Networking**: `pyngrok`, `requests`, `nest_asyncio`



## 🚀 실행 및 구성
1. 필요한 패키지를 설치합니다: `pip install flask flask-cors requests beautifulsoup4 pyngrok newspaper3k scikit-learn trafilatura`
2. `summanews_server(Gemini_API).ipynb` 파일을 실행합니다.
3. Ngrok을 통해 생성된 Public URL을 프론트엔드 앱의 API 주소로 설정합니다.

---

## 🔗 관련 프로젝트
- **Frontend**: [SummaNews-Frontend](https://github.com/seoyoung000/summanews-frontend) (React Native 기반 모바일 앱)
