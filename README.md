## Hi, I'm Taeyang 

I'm an AI Engineering student at Inha University with a strong interest in **World Models**, **Scene-Understanding**, **Video Generation** , **3D Reconstruction/4D Reconstruction (Gaussian Splatting)**, **Vision-Language-Action (VLA) models**, and **Multimodal AI**. Currently, I'm exploring World Models as an undergraduate researcher, focusing on how intelligent systems can learn and represent the dynamics of the world around them.

Beyond research, I enjoy turning ideas into systems that actually work. 
My recent projects span World Model, Scene Understanding, LLMs, RAG pipelines, multimodal applications, and practical deployment.

---

### What I'm working on

- Finishing up **RoboGuard**, an RLAIF-based RAG agent for industrial robot manuals that uses a self-correction loop (LangGraph + Gemini) to catch and fix hallucinated responses before they reach the user
- Exploring how inference-time defense strategies (like **B-VCD**) can make VLMs more reliable without any retraining

### Open-source contributions

- **[huggingface/transformers #51081](https://github.com/huggingface/transformers/pull/51081)** — added Qwen2-VL and Qwen2.5-VL GGUF files (llama.cpp) to the GGUF loading path, verified against the original model on a real 2B checkpoint *(under review)*
- **[kohya-ss/musubi-tuner #1171](https://github.com/kohya-ss/musubi-tuner/pull/1171)** — fixed LoRA dropout staying active in the samples generated during training (video/image LoRA trainer for Wan, HunyuanVideo and others), with a regression test *(under review)*
- **[Genesis-Embodied-AI/genesis-world #3907](https://github.com/Genesis-Embodied-AI/genesis-world/pull/3907)** — fixed the `Point` force field pushing particles away for a positive strength in the Genesis physics simulator for robotics and embodied AI, with an analytical test on CPU and Metal *(under review)*

---

### Tech I use regularly

**Language**
`Python` `C++` `C`

**ML / DL**
`PyTorch` `Hugging Face Transformers` `scikit-learn` `TensorFlow / Keras`

**LLM & RAG**
`LangChain` `LangGraph` `ChromaDB` `LangSmith`

**Vision**
`OpenCV` `PIL` 

**General**
`Git` `Jupyter` `Google Colab` `macOS (Apple Silicon)`

---

### Projects

**[2026 National Parks Satellite Monitoring AI Challenge](https://aifactory.space/ko/competitions/9306)**
Bi-temporal satellite change detection for new buildings and tree removal in Korean national parks, using model ensembles and polygon-based change localization. **1st place out of 136 teams on the private leaderboard.**

**[2026 INHA AI CHALLENGE](https://github.com/taeyang0505/2026-INHA-AI-CHALLENGE)**
Action-conditioned robot video generation using DynamiCrafter, 12-dimensional action encoding, cross-attention conditioning, and background stabilization.

**[RoboGuard-RLAIF](https://github.com/taeyang0505/RoboGuard-RLAIF)**
An enterprise RAG agent for UR10e robot technical support. The core idea: instead of just retrieving and generating, the system runs a judge model on every response and loops back to revise if it detects hallucinated content. Integrates InstructGPT-style reward modeling, Reflexion-style episodic memory, and Self-RAG critique tokens — all wired together in a cyclic LangGraph pipeline with a Streamlit UI and LangSmith tracing.

**[B-VCD: Mitigating Object Hallucination in VLMs](https://github.com/taeyang0505/B-VCD-Mitigating-Object-Hallucination-in-VLMs)**
Training-free, inference-time hallucination defense for VLMs. Perturbs the visual input with a physically-modeled degradation (motion blur + illumination attenuation + Poisson–Gaussian noise) and selects the most grounded answer via a degraded-image-grounded LLM-as-a-Judge (Gemini 2.5 Flash) on VizWiz-VQA.

**[Emotion-Aware Multimodal Chatbot](https://github.com/taeyang0505/Emotion_Aware_Multimodal_Chatbot_Project_Text_Image_and_Response_Generation)**
Combines BiLSTM + Attention for text emotion recognition with EfficientNet for image emotion, then fuses both modalities to generate context-aware responses.

**[Pneumonia Classification](https://github.com/taeyang0505/Pneumonia-Classification-Project)**
CNN-based chest X-ray classifier built with TensorFlow/Keras.

**[Forest Cover Classification](https://github.com/taeyang0505/Forest_Cover_Classification_Project)**
Multi-class tabular classification using tree-based and ensemble methods.

---

### Competition & Awards

**[2026 National Parks Satellite Monitoring AI Challenge](https://aifactory.space/ko/competitions/9306)**

**1st Place (Grand Prize)** in Topic 3: Facility Change Detection, among **136 teams**. Private leaderboard score: **0.7068898922**. Organized by the Korea National Park Service (hosted on AIFactory).
Detected newly built structures and tree removal as polygons from bi-temporal satellite image pairs (0.55–0.7 m/px). With no training data provided, built the training set from license-checked public aerial imagery and change-detection datasets, deriving labels from building outlines and a tree-canopy segmenter and adding synthetic change pairs. Trained change-detection models with EfficientNet/ConvNeXt encoders, gated pair-level presence for the F1 term, and tuned polygon post-processing and 8-view TTA (max aggregation) directly on the official metric.

**[2026 INHA AI Challenge](https://dacon.io/competitions/official/236736/overview/description)**

**4th Place (Excellence Award)**, among **216 participants**. Private score: **0.2162** (lower is better).<br>
[Project Repository](https://github.com/taeyang0505/2026-INHA-AI-Challenge)
Generated 16-frame robot videos from a single image and a 16-step joint-action sequence. Fine-tuned DynamiCrafter-512 (a 1.44B-parameter video diffusion UNet) with actions injected through zero-initialized cross-attention tokens (absolute joints + deltas), trained in four stages on a single 32 GB GPU (SDPA attention, 8-bit AdamW), and froze the background at inference to suppress diffusion jitter.

**[2026 SINCON](https://github.com/WSY129/SINCON_2026_GPT-GivePrizeTous)**

**3rd Place**, Private leaderboard score (RMSLE): **0.149321**. Inha University inter-club AI competition (SINSA · INCOM · NETers), hosted on Kaggle.
Forecast hourly subway boardings at 71 stations on Incheon Lines 1, 2 and 7 for July–October 2026 (123 days × 18 hourly slots, 157,194 predictions) in a single shot from data up to June 2026. Built a stacked ensemble of LightGBM, XGBoost, CatBoost and TabM trained on residuals over a seasonal baseline, validated with time-ordered 4-fold cross-validation, and added holiday and event corrections.

**[2026 INHA AX-EDU HACKERTON](https://github.com/taeyang0505/INHA-AX-EDU-Hackerton)**

**2nd Place (Top Excellence Award)**,Inha University AX-EDU Hackathon.
Built LOOKteracy, a webcam-based reading-literacy service that diagnoses how students understand a text from how they read it, not only from their answers. Implemented face-recognition login with blink-based liveness checks (face-api.js, MediaPipe) and in-browser eye tracking with 9-point calibration (WebGazer.js). Turned gaze data into teacher reports covering heatmaps, scanpath replay, per-word fixation metrics and five-area scores, plus concept-level diagnosis and suggested student groupings. Runs fully offline from a single HTML file, with no install and no generative AI required.


### Certifications

**IBM SkillsBuild**

[![Agentic AI with LangChain & LangGraph](https://img.shields.io/badge/Agentic%20AI%20%7C%20LangChain%20%26%20LangGraph-IBM%20SkillsBuild-054ADA?style=flat-square&logo=ibm&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Agentic%20AI%20with%20LangChain%20and%20LangGraph.pdf)

**DeepLearning.ai**

[![Retrieval Augmented Generation](https://img.shields.io/badge/Retrieval%20Augmented%20Generation-DeepLearning.ai-0B6E4F?style=flat-square&logo=coursera&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Retrieval%20Augmented%20Generation.png)
[![Agentic AI](https://img.shields.io/badge/Agentic%20AI-DeepLearning.ai-0B6E4F?style=flat-square)](https://github.com/taeyang0505/taeyang0505/blob/main/Agentic%20AI.png)

**Naver Boostcourse**

[![AI Basic 1](https://img.shields.io/badge/AI%20Basic%201-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_ai_basic_1.pdf)
[![AI Basic 2](https://img.shields.io/badge/AI%20Basic%202-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_ai_basic_2.pdf)
[![Computer Vision](https://img.shields.io/badge/Computer%20Vision-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_cv.pdf)
[![Deep Learning 1](https://img.shields.io/badge/Deep%20Learning%201-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_dl_1.pdf)
[![NLP](https://img.shields.io/badge/NLP-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_nlp.pdf)
[![Linear Algebra](https://img.shields.io/badge/Linear%20Algebra-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_linear_algebra.pdf)
[![Model Compression](https://img.shields.io/badge/Model%20Compression-Naver%20Boostcourse-03C75A?style=flat-square&logo=naver&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/boostcourse_model_compression.pdf)

**Codecademy**

[![ML / AI Engineer Career Path](https://img.shields.io/badge/ML%20%2F%20AI%20Engineer%20Career%20Path-Codecademy-1F4056?style=flat-square&logo=codecademy&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Machine%20Learning%3AAI%20Engineer%20Career%20Path.pdf)
[![DL with TensorFlow](https://img.shields.io/badge/Deep%20Learning%20with%20TensorFlow-Codecademy-1F4056?style=flat-square&logo=codecademy&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Build%20Deep%20Learning%20Models%20with%20TensorFlow%20Skill%20Path.pdf)
[![Intro to LLMs](https://img.shields.io/badge/Intro%20to%20LLMs-Codecademy-1F4056?style=flat-square&logo=codecademy&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Intro%20to%20Large%20Language%20Models%20(LLMs)%20Course.pdf)
[![NLP Course](https://img.shields.io/badge/Getting%20Started%20with%20NLP-Codecademy-1F4056?style=flat-square&logo=codecademy&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Getting%20Started%20with%20Natural%20Language%20Processing%20Course.pdf)
[![Data & Programming Foundations for AI](https://img.shields.io/badge/Data%20%26%20Programming%20Foundations%20for%20AI-Codecademy-1F4056?style=flat-square&logo=codecademy&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Data%20and%20Programming%20Foundations%20for%20AI%20Skill%20Path.pdf)


---

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/HuggingFace-FFD21F?style=flat-square&logo=huggingface&logoColor=black"/>
</p>
