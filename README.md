<div align="center">

# Hi, I'm Rashid 👋

### ML Engineer | Fintech & Generative AI

*Building production ML systems for financial services — from model training to Docker deployment*

[![Profile Views](https://komarev.com/ghpvc/?username=RaNurbekov&label=Profile%20views&color=0e75b6&style=flat)](https://github.com/RaNurbekov)
[![Telegram](https://img.shields.io/badge/Telegram-@Ytyglika-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Ytyglika)
[![Email](https://img.shields.io/badge/Email-nurbekovrashidjob@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:nurbekovrashidjob@gmail.com)

</div>

---

## 👨‍💻 About Me

I'm an ML Engineer focused on **Fintech products** and **Generative AI**. I specialize in the full development cycle: data analysis → model training & optimization → production deployment via FastAPI + Docker.

I don't just train models in Jupyter — I build reliable, interpretable and scalable ML pipelines ready for real business use.

**Core expertise:**
- 🏦 **Fintech ML** — credit scoring, fraud detection (GNN + classical ML), PFM transaction categorization
- 🤖 **LLM & RAG** — Fine-Tuning (LoRA/PEFT), RAG architectures, voice AI assistants
- ⚙️ **MLOps** — MLflow, Evidently AI, Kafka Streaming, A/B testing, Docker

---

## 🛠 Tech Stack

**Machine Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![PyG](https://img.shields.io/badge/PyTorch_Geometric-GNN-EE4C2C?style=for-the-badge)
![SHAP](https://img.shields.io/badge/SHAP-Explainable_AI-8A2BE2?style=for-the-badge)

**LLM & Voice AI**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logoColor=white)
![LoRA](https://img.shields.io/badge/PEFT_LoRA-Fine--Tuning-FF6B6B?style=for-the-badge)
![Whisper](https://img.shields.io/badge/Whisper_v3-STT-00A67E?style=for-the-badge)
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

## 💼 Projects

### 🔍 [fraud-gnn](https://github.com/RaNurbekov/fraud-gnn)
> **Fraud detection via transaction graph analysis using Graph Convolutional Networks**

Транзакции представлены как граф: 590K узлов, 493K рёбер. **GCN видит транзакцию в контексте её связей** — если карта участвовала в подозрительных операциях, модель "заражает" соседей подозрением. Именно так работают антифрод системы Visa и Mastercard. AUC-ROC: 0.78, Fraud Recall: 62%.

> 💡 **GNN vs LightGBM:** классический ML смотрит на транзакцию изолированно, GNN видит коллаборативный фрод через топологию графа.

`PyTorch Geometric` `GCNConv` `NetworkX` `FastAPI` `IEEE-CIS Dataset` `Graph ML`

---

### 🛡️ [fraud-detection-api](https://github.com/RaNurbekov/fraud-detection-api)
> **Hybrid real-time fraud detection microservice**

Двухслойная архитектура: **Redis Velocity Check** (защита от брутфорса) + **LightGBM** (поведенческие паттерны). Встроенный **A/B Testing Router** распределяет трафик 80/20 между Champion и Challenger моделями для безопасного тестирования гипотез в продакшне.

`LightGBM` `Redis Feature Store` `Docker Compose` `FastAPI` `A/B Testing` `Class Imbalance`

---

### 🏦 [credit-risk-api](https://github.com/RaNurbekov/credit-scoring-ml-api.)
> **Full MLOps pipeline for bank credit scoring — from Kaggle dataset to deployed REST API**

LightGBM обёрнут в FastAPI-микросервис. **MLflow Model Registry** — модель динамически загружается по RUN_ID. **SHAP TreeExplainer** — каждый отказ сопровождается топ-5 факторами решения (требование банковских регуляторов). **Evidently AI** — мониторинг Data Drift. Логирование каждого предсказания в SQLite.

🔗 [Live Demo](https://credit-scoring-ml-api.onrender.com/predict)

`LightGBM` `MLflow` `SHAP` `Evidently AI` `FastAPI` `Docker` `SQLite` `Render`

---

### 🌊 [kafka-fraud-streaming](https://github.com/RaNurbekov/kafka-fraud-streaming)
> **Real-time fraud detection streaming pipeline on Apache Kafka**

Event-Driven пайплайн: Producer генерирует поток транзакций → Kafka Broker → Consumer Group с детектором. Демонстрация **горизонтального масштабирования** — при запуске нескольких Consumer инстансов Kafka автоматически перераспределяет нагрузку (Rebalance).

`Apache Kafka` `Zookeeper` `Docker Compose` `Consumer Groups` `Event-Driven`

---

### 💬 [bank-ai-assistant](https://github.com/RaNurbekov/llm_bot-ai_bank_assistant-)
> **Intelligent bank support assistant with semantic search over knowledge base (RAG)**

Полноценная **RAG-архитектура**: документы → чанкинг → HuggingFace Embeddings → **Qdrant** (векторная БД) → Llama 3 (Groq). Жёсткий Hallucination Prevention: бот отвечает строго по документам, показывая источники через Expander UI.

`Qdrant` `RAG` `LangChain` `Llama-3` `HuggingFace Embeddings` `Streamlit`

---

### 🎙️ [voice-bank-assistant](https://github.com/RaNurbekov/ai_voice_assistant)
> **Full voice pipeline: Speech-to-Text → LLM → Text-to-Speech with conversation memory**

Полный голосовой пайплайн: **Whisper Large v3** транскрибирует речь → **Llama 3.3-70B** генерирует ответ с памятью всего диалога → **gTTS** синтезирует голос с автовоспроизведением. System Prompt оптимизирован под TTS-сценарий: краткие ответы без списков, как живой оператор по телефону.

`Whisper v3` `Llama-3.3-70B` `gTTS` `Groq` `Conversation Memory` `Streamlit`

---

### 🧠 [bank-llm-finetuning](https://github.com/RaNurbekov/bank-llm-finetuning)
> **Parameter-Efficient Fine-Tuning of LLM for bank support (PEFT/LoRA)**

Fine-Tuning **TinyLlama-1.1B** с использованием **LoRA-адаптеров** — обучалось всего **1,126,400 параметров (0.10%)** вместо полной модели. Cloud-to-Local Pipeline: обучение на GPU (Google Colab T4) → инференс на CPU.

> 💡 **RAG vs Fine-Tuning:** `bank-ai-assistant` использует внешнюю базу знаний, этот проект "зашивает" знания в веса модели — два подхода к одной задаче.

`TinyLlama` `LoRA` `PEFT` `SFTTrainer` `PyTorch` `HuggingFace`

---

### 💳 [bank-transaction-categorizer](https://github.com/RaNurbekov/Transaction-Categorizer-Deep-Learning-PyTorch-Hugging-Face-NLP-)
> **NLP system for "dirty" bank transaction categorization (PFM)**

Fine-Tuning многоязычного **DistilBERT** на классификацию 5 банковских категорий. Модель устойчива к опечаткам, латинице и шумам (ID терминалов). Inference UI с Confidence Score на Streamlit.

`DistilBERT` `PyTorch` `Hugging Face` `Fine-Tuning` `NLP` `Streamlit`

---

### 🔥 [pytorch-bank-churn](https://github.com/RaNurbekov/pytorch-bank-churn)
> **Bank churn prediction with custom PyTorch MLP from scratch**

Полносвязная нейросеть (MLP) реализована на **чистом PyTorch** без высокоуровневых оберток. Ручная реализация Training Loop, Forward/Backward Pass, `DataLoader` с батч-обработкой тензоров. Accuracy: **94.5%** на тестовой выборке.

`PyTorch` `MLP` `Custom Training Loop` `Binary Classification`

---

### 👁️ [yolov8-object-detection](https://github.com/RaNurbekov/computer_vision_simple_sample)
> **Real-time object detection web application (YOLOv8)**

Zero-Shot Inference на предобученных весах MS COCO (80 классов). Поддержка масштабирования от `yolov8n` (Nano) до `yolov8x` (eXtra Large). Автоматический парсинг Bounding Boxes и генерация статистики.

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

## 📫 Get in Touch

| | |
|---|---|
| 📧 Email | [nurbekovrashidjob@gmail.com](mailto:nurbekovrashidjob@gmail.com) |
| 💬 Telegram | [@RaNurbek](https://t.me/@RaNurbek) |
| 📍 Location | Almaty, Kazakhstan 🇰🇿 |

---

<div align="center">
  <i>"Data without action is just numbers. I build systems that make decisions."</i>
</div>
