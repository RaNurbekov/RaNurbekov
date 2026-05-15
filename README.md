<div align="center">

# Привет, я Рашид 👋

### Junior ML Engineer | Fintech & Generative AI

<div align="center">

# Привет, я Рашид 👋

### ML Engineer | Fintech & Generative AI

*Строю ML-сервисы для финтеха — от обучения модели до деплоя в Docker*

[![Profile Views](https://komarev.com/ghpvc/?username=RaNurbekov&label=Profile%20views&color=0e75b6&style=flat)](https://github.com/RaNurbekov)
[![Telegram](https://img.shields.io/badge/Telegram-@Ytyglika-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Ytyglika)
[![Email](https://img.shields.io/badge/Email-nurbekovrashidjob@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:nurbekovrashidjob@gmail.com)

</div>

---

## 👨‍💻 Обо мне

Я ML-инженер с фокусом на **финтех-продукты** и **Generative AI**. Специализируюсь на полном цикле разработки: глубокий анализ данных → обучение и оптимизация моделей → production-деплой через FastAPI + Docker.

Не просто обучаю модели в Jupyter — строю надёжные, интерпретируемые и масштабируемые пайплайны, готовые к реальному бизнесу.

**Ключевые области:**
- 🏦 **Fintech ML** — кредитный скоринг, антифрод, PFM-категоризация транзакций
- 🤖 **LLM & RAG** — Fine-Tuning (LoRA/PEFT), RAG-архитектуры, AI-агенты банковской поддержки
- ⚙️ **MLOps** — MLflow, Evidently AI, Kafka Streaming, A/B тестирование, Docker

---

## 🛠 Технологический стек

**Machine Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![SHAP](https://img.shields.io/badge/SHAP-Explainable_AI-8A2BE2?style=for-the-badge)

**LLM & Fine-Tuning**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logoColor=white)
![LoRA](https://img.shields.io/badge/PEFT_LoRA-Fine--Tuning-FF6B6B?style=for-the-badge)
![Groq](https://img.shields.io/badge/Groq_API_(Llama_3)-F55036?style=for-the-badge&logoColor=white)

**Backend & MLOps**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![Evidently](https://img.shields.io/badge/Evidently_AI-Data_Drift-6C3483?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

---

## 💼 Портфолио

### 🛡️ [fraud-detection-api](https://github.com/RaNurbekov/fraud-detection-api)
> **Гибридная микросервисная система детектирования мошенничества в реальном времени**

Двухслойная архитектура: **Redis Velocity Check** (защита от брутфорса) + **LightGBM** (поведенческие паттерны). Встроенный **A/B Testing Router** распределяет трафик 80/20 между Champion и Challenger моделями для безопасного тестирования гипотез в продакшне.

`LightGBM` `Redis Feature Store` `Docker Compose` `FastAPI` `A/B Testing` `Class Imbalance`

---

### 🏦 [credit-risk-api](https://github.com/RaNurbekov/credit-scoring-ml-api.)
> **Полный MLOps-цикл кредитного скоринга: от Kaggle-датасета до задеплоенного REST API**

LightGBM обёрнут в FastAPI-микросервис. **MLflow Model Registry** — модель динамически загружается по RUN_ID без изменения кода. **SHAP TreeExplainer** — каждый отказ сопровождается топ-5 факторами решения (требование банковских регуляторов). **Evidently AI** — мониторинг Data Drift. Логирование каждого предсказания в SQLite.

🔗 [Live Demo](https://credit-scoring-ml-api.onrender.com/predict)

`LightGBM` `MLflow` `SHAP` `Evidently AI` `FastAPI` `Docker` `SQLite` `Render`

---

### 🌊 [kafka-fraud-streaming](https://github.com/RaNurbekov/kafka_anti_fraud)
> **Потоковая архитектура для обнаружения мошенничества на Apache Kafka**

Event-Driven пайплайн: Producer генерирует поток транзакций → Kafka Broker → Consumer Group с детектором. Демонстрация **горизонтального масштабирования** — при запуске нескольких Consumer инстансов Kafka автоматически перераспределяет нагрузку (Rebalance). Готов к интеграции с `fraud-detection-api` для ML-инференса.

`Apache Kafka` `Zookeeper` `Docker Compose` `Consumer Groups` `Event-Driven`

---

### 💬 [bank-ai-assistant](https://github.com/RaNurbekov/llm_bot-ai_bank_assistant-)
> **Интеллектуальный консультант с семантическим поиском по корпоративной базе знаний**

Полноценная **RAG-архитектура**: документы → чанкинг → HuggingFace Embeddings → **Qdrant** (векторная БД) → Llama 3 (Groq). Жёсткий Hallucination Prevention: бот отвечает строго по документам, показывая источники через Expander UI.

`Qdrant` `RAG` `LangChain` `Llama-3` `HuggingFace Embeddings` `Streamlit`

---

### 🧠 [bank-llm-finetuning](https://github.com/RaNurbekov/bank_llm_finetuning)
> **Parameter-Efficient Fine-Tuning LLM для банковской поддержки (PEFT/LoRA)**

Fine-Tuning **TinyLlama-1.1B** с использованием **LoRA-адаптеров** — обучалось всего **1,126,400 параметров (0.10%)** вместо полной модели. Cloud-to-Local Pipeline: обучение на GPU (Google Colab T4) → инференс на CPU через `PeftModel`. Честный разбор Lessons Learned: Underfitting, галлюцинации и пути к production-качеству.

> 💡 **RAG vs Fine-Tuning:** `bank-ai-assistant` использует внешнюю базу знаний (RAG), этот проект "зашивает" знания в веса модели (Fine-Tuning) — два подхода к одной задаче.

`TinyLlama` `LoRA` `PEFT` `SFTTrainer` `PyTorch` `HuggingFace` `Google Colab`

---

### 💳 [bank-transaction-categorizer](https://github.com/RaNurbekov/Transaction-Categorizer-Deep-Learning-PyTorch-Hugging-Face-NLP-)
> **NLP-система категоризации "грязных" банковских транзакций (PFM)**

Fine-Tuning многоязычного **DistilBERT** на классификацию 5 банковских категорий. Модель устойчива к опечаткам, латинице и шумам (ID терминалов). Inference UI с Confidence Score на Streamlit.

`DistilBERT` `PyTorch` `Hugging Face` `Fine-Tuning` `NLP` `Streamlit`

---

### 👁️ [yolov8-object-detection](https://github.com/RaNurbekov/computer_vision_simple_sample)
> **Веб-приложение для детектирования объектов в реальном времени**

Zero-Shot Inference на предобученных весах MS COCO (80 классов). Поддержка масштабирования от `yolov8n` (Nano, real-time) до `yolov8x` (eXtra Large). Автоматический парсинг Bounding Boxes и генерация статистики.

`YOLOv8` `Ultralytics` `OpenCV` `Zero-Shot` `Streamlit`

---

## 📊 GitHub Stats

<div align="center">

![RaNurbekov's GitHub Stats](https://github-readme-stats.vercel.app/api?username=RaNurbekov&show_icons=true&theme=dark&hide_border=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=RaNurbekov&layout=compact&theme=dark&hide_border=true)

</div>

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com?user=RaNurbekov&theme=dark&hide_border=true)

</div>

---

## 📫 Связаться со мной

| | |
|---|---|
| 📧 Email | [nurbekovrashidjob@gmail.com](mailto:nurbekovrashidjob@gmail.com) |
| 💬 Telegram | [@Ytyglika](https://t.me/Ytyglika) |
| 📍 Локация | Алматы, Казахстан 🇰🇿 |

---

<div align="center">
  <i>"Данные без действия — это просто числа. Я строю системы, которые принимают решения."</i>
</div>
