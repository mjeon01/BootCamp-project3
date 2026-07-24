# 🌿 AI Bootcamp Project 3 - AI 공감 다이어리

> **한 줄의 일기를 입력하면 AI가 감정을 분석하고 공감 메시지를 생성해주는 웹 서비스**

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white">
  <img src="https://img.shields.io/badge/OpenAI-GPT--4o--mini-412991?style=for-the-badge&logo=openai&logoColor=white">
</p>

---

# 📌 Project Overview

AI 공감 다이어리는 사용자가 하루를 한 줄로 기록하면 OpenAI GPT 모델을 활용하여

- 감정을 분석하고
- 대표 감정을 분류하며
- 따뜻한 공감 및 위로 메시지를 생성하는 서비스입니다.

복잡한 기능보다는 **감정 분석 + 공감 생성**에 집중한 간단한 AI 서비스입니다.

---

# ✨ Features

### 📝 한 줄 일기 작성

- 오늘 있었던 일을 자유롭게 입력

---

### 😊 감정 분석

AI가 입력 내용을 분석하여 아래 8가지 감정 중 하나로 분류합니다.

- 😊 기쁨
- 🥰 설렘
- 🙂 평온
- 😢 슬픔
- 😟 불안
- 😠 분노
- 😮‍💨 지침
- 🌫 기타

---

### 💌 공감 메시지 생성

GPT가 상황에 맞는

- 공감
- 위로
- 감정 인정

메시지를 자연스럽게 생성합니다.

---

### 📖 기록 관리

작성한 일기는

- 최신순으로 조회
- 삭제 가능

세션 동안 유지됩니다.

---

### 🛡 예외 처리

OpenAI API를 사용할 수 없는 경우

- 기본 공감 메시지 출력
- 앱은 정상 동작 유지

---

# 🏗️ Project Structure

```
project3/
│
├── app.py                # Streamlit 메인 애플리케이션
├── requirements.txt      # 프로젝트 의존성
├── .env                  # OpenAI API Key (로컬)
├── .streamlit/
│     └── secrets.toml    # Streamlit Cloud Secret
│
└── README.md
```

---

# ⚙️ Tech Stack

| Category | Technology |
|-----------|------------|
| Language | Python |
| Web | Streamlit |
| AI Model | OpenAI GPT-4o-mini |
| API | OpenAI API |
| Environment | python-dotenv |
| Deployment | Streamlit Cloud |

---

# 🔄 Workflow

```
사용자 입력
      │
      ▼
한 줄 일기 작성
      │
      ▼
OpenAI GPT-4o-mini
      │
      ├──────────────┐
      ▼              ▼
감정 분류        공감 메시지 생성
      │              │
      └──────┬───────┘
             ▼
      결과 화면 출력
             │
             ▼
      기록 저장(Session)
```

---

# 🚀 Installation

## 1. Clone Repository

```bash
git clone https://github.com/your-repository.git
cd project3
```

---

## 2. Install Packages

```bash
pip install -r requirements.txt
```

---

## 3. Set API Key

### 방법 1 (.env)

```env
OPENAI_API_KEY=your_api_key
```

---

### 방법 2 (Streamlit Cloud)

```
OPENAI_API_KEY=your_api_key
```

Secrets에 등록하면 됩니다.

---

## 4. Run

```bash
streamlit run app.py
```

---

# 💻 Example

### 입력

```
오늘 시험을 망쳐서 너무 속상했다.
```

---

### 출력

**감정**

```
😢 슬픔
```

**공감 메시지**

```
오늘 하루가 많이 힘들었겠어요.
시험 결과 하나만으로 당신의 노력이 사라지는 것은 아닙니다.
지금 느끼는 속상함도 충분히 자연스러운 감정입니다.
```

---

# 📦 Requirements

```
streamlit
openai
python-dotenv
```

또는

```bash
pip install -r requirements.txt
```

---

# 📌 Future Improvements

- 로그인 기능
- 데이터베이스 저장
- 감정 통계
- 감정 변화 그래프
- 감정 캘린더
- 음성 일기 입력
- 이미지 기반 감정 분석
- 다국어 지원

---

# 👨‍💻 Author

**AI Bootcamp Project 3**

AI Empathy Diary
