<h1 align="center">Ekaghni Mukherjee</h1>

<p align="center">
  ML engineer who started out on Android.<br>
  I build and train models, then get them running in production.
</p>

<p align="center">
  <a href="mailto:ekaghni.mukherjee@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://www.linkedin.com/in/ekaghni-mukherjee-8a1446210"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square" alt="LinkedIn"></a>
</p>

## About

I work as an R&D Machine Learning Engineer at Telaverge Communications. My job covers the whole life of a model. I pick the approach, build it, train it, tune it, and then get it running in production.

On the modelling side that has meant LSTMs with attention for log anomaly detection, VAEs and graph autoencoders for representation learning, DQN agents with prioritized replay, CNNs for vision, and gradient boosting or Isolation Forest when the data is tabular. On the LLM side I build RAG systems, serve open models on vLLM and wire up agent workflows.

Before ML I spent over a year building Android apps at Cre Innovations. Style transfer, face swap and photo editing, all of it running on the phone GPU through OpenGL ES, the NDK and FFmpeg. That job taught me to think about memory and latency first, and I still build ML systems that way.

I also like writing things from scratch to see how they work inside. So far that list has a transformer, Stable Diffusion and a DQN agent that learned to race.

## What I work on

- **Classical ML.** Isolation Forest, decision trees and ensembles for anomaly detection. XGBoost, LightGBM and CatBoost for tabular problems, with Optuna and Hyperopt for tuning. A lot of feature engineering on time-series logs using statistical measures, n-grams and temporal patterns.
- **Deep learning.** CNNs with transfer learning from ResNet and EfficientNet. LSTMs with attention for sequence tasks and forecasting. VAEs for latent space interpolation and graph autoencoders for unsupervised representation learning. Transformers built from the ground up with RoPE, SwiGLU and RMSNorm.
- **Reinforcement learning.** DQN, Double DQN and Dueling DQN with prioritized experience replay, target networks and curriculum learning.
- **Generative models.** Stable Diffusion written from its parts (CLIP, U-Net, VAE). LoRA fine-tuning of Flux Kontext for controlled image generation.
- **LLM applications.** RAG with hybrid retrieval using BM25 and dense embeddings. Getting recall up was the easy part. Most of the effort went into re-ranking and context compression so the model stops making things up. Multi-agent workflows in LangGraph with tool calling and conditional routing.
- **Serving and MLOps.** Llama 3.2, Qwen 2.5 Coder and LLaVA 1.6 behind OpenAI compatible APIs on vLLM. ONNX export, Docker, model versioning, A/B tests and CI/CD rollouts. Runs tracked in Weights & Biases and MLflow.
- **On-device graphics.** OpenGL ES pipelines, GLSL shaders and NDK code for image processing that has to hold 60 FPS.

## Projects

| Project | What it does | Built with |
|---|---|---|
| [DQN Racing Agent](https://github.com/Ekaghni/DQN-Reinforcement-Learning-Car-Model) | A Dueling Double DQN that learns to drive seven tracks using 15 ray-cast sensors. I wrote the physics simulation myself. It gets past 85% track completion with no expert demonstrations. | PyTorch, PyGame |
| HelpSteer Transformer | A 60M parameter transformer with RoPE, SwiGLU and RMSNorm. Learned embeddings give control over five response attributes. Runs at 4,200 tokens per second. | PyTorch |
| Stable Diffusion from scratch | The CLIP text encoder, U-Net and VAE decoder written by hand instead of pulled from a library. Mixed precision and attention slicing cut VRAM use by about half. | PyTorch, Gradio |
| Face Mesh Retouch | Real-time face retouching on Android with MediaPipe landmarks and custom GLSL shaders. The C++ render path runs about 3x faster than the Java one. | OpenGL ES 3.0, NDK |
| Log Anomaly Detection | Isolation Forest over server logs with real-time alerts. It brought mean time to detection down by around 60% in production. | scikit-learn, MLflow |
| [Sentiment Analysis](https://github.com/Ekaghni/sentiment_analysis_project) | Scores comments with VADER and a RoBERTa model and sends an email alert when the sentiment shifts. Served through a Django REST API. | NLTK, Transformers, Django |
| Skin Cancer Classifier | A multi-class classifier trained on a small dermatology dataset. Transfer learning from ResNet and EfficientNet, weighted loss for class imbalance, and attention maps so the predictions can be checked. | PyTorch |

Some of my earlier Android work is here too. [Firebase Firestore CRUD with auth and notifications](https://github.com/Ekaghni/Firebase-Firestore-CRUD-Auth-Notification), [Retrofit with SQLite and Gson](https://github.com/Ekaghni/Retrofit-SQLite-Gson-App) and an [anime web scraper](https://github.com/Ekaghni/Anime-Web-Scrapper).

## Tools

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square)

**Machine learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-2F8F4E?style=flat-square)
![CatBoost](https://img.shields.io/badge/CatBoost-FFCC00?style=flat-square)
![Optuna](https://img.shields.io/badge/Optuna-1F4E9E?style=flat-square)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-111F68?style=flat-square)
![Stable-Baselines3](https://img.shields.io/badge/Stable--Baselines3-4B6CB7?style=flat-square)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)

**LLMs**

![Transformers](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![LlamaIndex](https://img.shields.io/badge/LlamaIndex-7B3FE4?style=flat-square)
![vLLM](https://img.shields.io/badge/vLLM-30A2FF?style=flat-square)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-E9573F?style=flat-square)

**Deployment**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![Weights and Biases](https://img.shields.io/badge/W%26B-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Android**

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![OpenGL ES](https://img.shields.io/badge/OpenGL%20ES-5586A4?style=flat-square&logo=opengl&logoColor=white)
![NDK](https://img.shields.io/badge/NDK-3DDC84?style=flat-square)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white)
![RxJava](https://img.shields.io/badge/RxJava-B7178C?style=flat-square)
![Retrofit](https://img.shields.io/badge/Retrofit-48B983?style=flat-square)

## Background

- R&D Machine Learning Engineer at Telaverge Communications, 2024 to now
- Software Engineer Intern at Telaverge Communications, 2023 to 2024
- Android Developer at Cre Innovations, 2022 to 2023
- B.Tech in Computer Science and Engineering from MAKAUT, 2024

## Get in touch

Email is the fastest way to reach me. I am always up for a conversation about LLM serving, retrieval that does not hallucinate, or squeezing image processing onto a phone.
