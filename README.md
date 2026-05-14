<div align="center">

# Привет, я Рашид 👋

### Junior ML Engineer | Fintech & Generative AI

*Строю ML-сервисы для финтеха — от обучения модели до деплоя в Docker*

[![Profile Views](https://komarev.com/ghpvc/?username=RaNurbekov&label=Profile%20views&color=0e75b6&style=flat)](https://github.com/RaNurbekov)
[![Telegram](https://img.shields.io/badge/Telegram-@Ytyglika-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Ytyglika)
[![Email](https://img.shields.io/badge/Email-nurbekovrashidjob@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:nurbekovrashidjob@gmail.com)

</div>

---

## 👨‍💻 Обо мне

Я Начинающий ML-инженер с фокусом на **финтех-продукты** и **Generative AI**. Специализируюсь на полном цикле разработки: глубокий анализ данных → обучение и оптимизация моделей → production-деплой через FastAPI + Docker.

Не просто обучаю модели в Jupyter — строю надёжные, интерпретируемые и масштабируемые пайплайны, готовые к реальному бизнесу.

**Ключевые области:**
- 🏦 **Fintech ML** — кредитный скоринг, антифрод, PFM-категоризация транзакций
- 🤖 **LLM & RAG** — разработка AI-агентов и интеллектуальных ботов поддержки
- ⚙️ **MLOps** — CI/CD для моделей, мониторинг Data Drift, A/B тестирование

---

## 🛠 Технологический стек

**Machine Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![SHAP](https://img.shields.io/badge/SHAP-Explainable_AI-8A2BE2?style=for-the-badge)

**LLM & Vector Search**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logoColor=white)
![Groq](https://img.shields.io/badge/Groq_API_(Llama_3)-F55036?style=for-the-badge&logoColor=white)

**Backend & DevOps**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

---

## 💼 Портфолио

### 🛡️ [Anti-Fraud Transaction API](https://github.com/RaNurbekov/fraud-detection-api)
> **Гибридная микросервисная система детектирования мошенничества в реальном времени**

Двухслойная архитектура: Redis Velocity Check (защита от брутфорса) + LightGBM (поведенческие паттерны). Встроенный **A/B Testing Router** распределяет трафик 80/20 между Champion и Challenger моделями для безопасного тестирования гипотез в продакшне.

`LightGBM` `Redis Feature Store` `Docker Compose` `FastAPI` `A/B Testing` `Class Imbalance`

---

### 🏦 [Credit Risk API](https://github.com/RaNurbekov/credit-risk-api)
> **Полный цикл кредитного скоринга: от Kaggle-датасета до задеплоенного REST API**

Модель LightGBM обёрнута в FastAPI-микросервис с Docker. Реализован **Explainable AI (SHAP)** — каждый отказ по кредиту сопровождается топ-5 факторов принятия решения. Логирование каждого предсказания в SQLite. Live API задеплоен на Render.

🔗 [Live Demo](https://credit-scoring-ml-api.onrender.com/predict)

`LightGBM` `SHAP` `FastAPI` `Docker` `SQLite` `Render`

---

### 💬 [Bank AI Assistant (True RAG)](https://github.com/RaNurbekov/bank-ai-assistant)
> **Интеллектуальный консультант с семантическим поиском по корпоративной базе знаний**

Полноценная RAG-архитектура: документы → чанкинг → HuggingFace Embeddings → **Qdrant** (векторная БД) → Llama 3 (Groq). Жёсткий Hallucination Prevention: бот отвечает строго по документам, показывая источники через Expander.

`Qdrant` `RAG` `LangChain` `Llama-3` `HuggingFace Embeddings` `Streamlit`

---

### 💳 [Bank Transaction Categorizer](https://github.com/RaNurbekov/bank-transaction-categorizer)
> **NLP-система категоризации "грязных" банковских транзакций (PFM)**

Fine-Tuning многоязычного **DistilBERT** (Hugging Face) на задачу классификации 5 банковских категорий. Модель устойчива к опечаткам, латинице и шумам (ID терминалов). Inference UI с Confidence Score на Streamlit.

`DistilBERT` `PyTorch` `Hugging Face` `Fine-Tuning` `NLP` `Streamlit`

---

### 👁️ [YOLOv8 Object Detection](https://github.com/RaNurbekov/yolov8-object-detection)
> **Веб-приложение для видеоаналитики и детектирования объектов в реальном времени**

Zero-Shot Inference на предобученных весах MS COCO (80 классов). Поддержка масштабирования от `yolov8n` (Nano, real-time) до `yolov8x` (eXtra Large). Автоматический парсинг Bounding Boxes и генерация бизнес-статистики.

`YOLOv8` `Ultralytics` `OpenCV` `Zero-Shot` `Streamlit`

---

## 📊 GitHub Stats

<div align="center">

![RaNurbekov's GitHub Stats](https://github-readme-stats.vercel.app/api?username=RaNurbekov&show_icons=true&theme=dark&hide_border=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=RaNurbekov&layout=compact&theme=dark&hide_border=true)

</div>

---

## 📫 Связаться со мной

| | |
|---|---|
| 📧 Email | [nurbekovrashidjob@gmail.com](mailto:nurbekovrashidjob@gmail.com) |
| 💬 Telegram | [@Ytyglika](https://t.me/Ytyglika) |
| 📍 Локация | Алматы, Казахстан |

---

<div align="center">
  <i>"Данные без действия — это просто числа. Я строю системы, которые принимают решения."</i>
</div>
