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
- 🏦 **Fintech ML** — credit scoring, fraud detection (GNN + classical ML), PFM analytics
- 🤖 **LLM & Agents** — Fine-Tuning (LoRA/PEFT), RAG, Voice AI, LangGraph ReAct Agents
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
![LangGraph](https://img.shields.io/badge/LangGraph-ReAct_Agent-1C3C3C?style=for-the-badge)
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

🔗 [API](https://fraud-gnn-1.onrender.com) | [Graph Visualizer](https://fraud-gnn-j6nh9vg4mb4tdabnshx2n3.streamlit.app)

`PyTorch Geometric` `GCNConv` `NetworkX` `FastAPI` `Streamlit` `Render`

---

### 🛡️ [fraud-detection-api](https://github.com/RaNurbekov/fraud-detection-api)
> **Hybrid real-time fraud detection microservice**

Двухслойная архитектура: **Redis Velocity Check** (защита от брутфорса) + **LightGBM** (поведенческие паттерны). Встроенный **A/B Testing Router** распределяет трафик 80/20 между Champion и Challenger моделями.

🔗 [Live API](https://fraud-detection-api-1-hf78.onrender.com)

`LightGBM` `Redis Feature Store` `Docker Compose` `FastAPI` `A/B Testing` `Render`

---

### 🏦 [credit-risk-api](https://github.com/RaNurbekov/credit-scoring-ml-api.)
> **Full MLOps pipeline for bank credit scoring — from Kaggle dataset to deployed REST API**

LightGBM + FastAPI. **MLflow Model Registry** — динамическая загрузка модели по RUN_ID. **SHAP** — топ-5 факторов решения. **Evidently AI** — мониторинг Data Drift. SQLite аудит-лог.

🔗 [Live API](https://credit-scoring-ml-api.onrender.com/predict)

`LightGBM` `MLflow` `SHAP` `Evidently AI` `FastAPI` `Docker` `Render`

---

### 💰 [pfm-ai-assistant](https://github.com/RaNurbekov/pfm_ai_assistant)
> **End-to-end AI Personal Finance Manager — localized for Kazakhstan 🇰🇿**

NLP категоризация транзакций → Anomaly Detection → Prophet Forecast → Voice Assistant → PDF Reports → Telegram Bot. Симуляция KZ клиентов (Glovo, Kaspi, inDrive). Мультивалютность (8 валют).

🔗 [Live Demo](https://pfm-ai-assistant.streamlit.app)

`Prophet` `Evidently AI` `Whisper` `Llama-3` `Telegram Bot` `Streamlit`

---

### 🌊 [kafka-fraud-streaming](https://github.com/RaNurbekov/kafka-fraud-streaming)
> **Real-time fraud detection streaming pipeline on Apache Kafka**

Event-Driven пайплайн: Producer → Kafka Broker → Consumer Group → **LightGBM ML API**. Consumer вызывает `fraud-detection-api` для реального ML инференса вместо Rule-Based логики.

`Apache Kafka` `Zookeeper` `Docker Compose` `Consumer Groups` `ML Integration`

---

### 🤖 [financial-ai-agent](https://github.com/RaNurbekov/financial-advisor-bot)
> **Autonomous Financial AI Agent with 5 tools (LangGraph ReAct)**

LangGraph ReAct агент с инструментами: DuckDuckGo Search, Loan Calculator, Deposit Calculator, Currency Converter, Fraud Risk Checker. Сам решает какой инструмент вызвать.

🔗 [Live Demo](https://financial-advisor-bot-ilewnbcmhlsk5i2kote5xr.streamlit.app)

`LangGraph` `LangChain` `Llama-3.3-70B` `Tool Calling` `Groq` `Streamlit`

---

### 💬 [bank-ai-assistant](https://github.com/RaNurbekov/bank-ai-assistant)
> **Intelligent bank support assistant with semantic search over knowledge base (RAG)**

Полноценная **RAG-архитектура**: документы → чанкинг → HuggingFace Embeddings → **Qdrant** → Llama 3. Hallucination Prevention: бот отвечает строго по документам.

🔗 [Live Demo](https://bank-ai-assistant-82mcu6adkv2vqviwhpzft6.streamlit.app)

`Qdrant` `RAG` `LangChain` `Llama-3` `HuggingFace Embeddings` `Streamlit`

---

### 🎙️ [voice-bank-assistant](https://github.com/RaNurbekov/ai_voice_assistant)
> **Full voice pipeline: Speech-to-Text → LLM → Text-to-Speech**

**Whisper Large v3** → **Llama 3.3-70B** → **gTTS**. Память всего диалога. System Prompt оптимизирован под TTS: краткие ответы как живой оператор по телефону.

🔗 [Live Demo](https://aivoiceassistant-9uqgi56eevhbe266yyntfz.streamlit.app)

`Whisper v3` `Llama-3.3-70B` `gTTS` `Groq` `Conversation Memory` `Streamlit`

---

### 🧠 [bank-llm-finetuning](https://github.com/RaNurbekov/bank-llm-finetuning)
> **Parameter-Efficient Fine-Tuning of LLM for bank support (PEFT/LoRA)**

Fine-Tuning **TinyLlama-1.1B** — обучалось **1,126,400 параметров (0.10%)**. Cloud-to-Local Pipeline: Colab T4 GPU → CPU inference. Streamlit Chat UI.

🔗 [Live Demo](https://bank-llm-finetuning.streamlit.app)

`TinyLlama` `LoRA` `PEFT` `SFTTrainer` `PyTorch` `HuggingFace`

---

### 💳 [bank-transaction-categorizer](https://github.com/RaNurbekov/Transaction-Categorizer-Deep-Learning-PyTorch-Hugging-Face-NLP-)
> **NLP system for "dirty" bank transaction categorization (PFM)**

Fine-Tuning многоязычного **DistilBERT** на 5 банковских категорий. Устойчив к опечаткам, латинице и шумам POS-терминалов. Confidence Score UI.

`DistilBERT` `PyTorch` `Hugging Face` `Fine-Tuning` `NLP` `Streamlit`

---

### 🔥 [pytorch-bank-churn](https://github.com/RaNurbekov/pytorch-bank-churn)
> **Bank churn prediction — custom PyTorch MLP from scratch | ROC-AUC: 0.9685**

Кастомный Training Loop на чистом PyTorch. BatchNorm + Dropout. Обучен на реальном датасете (10,127 клиентов). Бизнес-рекомендации по уровню риска.

🔗 [Live Demo](https://pytorch-bank-churn-eopnllazuzaixg9rlwbuvh.streamlit.app)

`PyTorch` `MLP` `BatchNorm` `ROC-AUC 0.97` `Streamlit`

---

### 👁️ [yolov8-object-detection](https://github.com/RaNurbekov/-yolov8-object-detection)
> **Real-time object detection web application (YOLOv8)**

Zero-Shot Inference на MS COCO (80 классов). Выбор модели от Nano до XLarge. Confidence slider. Plotly analytics dashboard.

🔗 [Live Demo](https://5jqwsy2zmlp6dmztnkhtwk.streamlit.app)

`YOLOv8` `Ultralytics` `OpenCV` `Zero-Shot` `Plotly` `Streamlit`

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
| 💬 Telegram | [@Ytyglika](https://t.me/Ytyglika) |
| 📍 Location | Almaty, Kazakhstan 🇰🇿 |

---

<div align="center">
  <i>"Data without action is just numbers. I build systems that make decisions."</i>
</div>
