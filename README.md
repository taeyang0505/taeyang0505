## Hi, I'm Taeyang 👋

I'm an AI Engineering student at Inha University with a strong interest in **Computer Vision** and **Multimodal AI**. I've spent the last year digging into Vision-Language Models (VLMs) as an undergraduate research assistant — specifically on the problem of object hallucination, where models confidently describe things that aren't in the image.

Beyond research, I like building things that actually run. Most of my recent projects sit at the intersection of LLMs, RAG pipelines, and practical deployment.

---

### What I'm working on

- Finishing up **RoboGuard**, an RLAIF-based RAG agent for industrial robot manuals that uses a self-correction loop (LangGraph + Gemini) to catch and fix hallucinated responses before they reach the user
- Exploring how inference-time defense strategies (like **B-VCD**) can make VLMs more reliable without any retraining

### Open-source contributions

- **[kubeflow/mcp-server #44](https://github.com/kubeflow/mcp-server/pull/44)** — added HuggingFace model-ID suggestions to the MCP server's `pre_flight` tool, with unit tests *(under review)*

---

### Tech I use regularly

**ML / DL**
`PyTorch` `Hugging Face Transformers` `scikit-learn` `TensorFlow / Keras`

**LLM & RAG**
`LangChain` `LangGraph` `ChromaDB` `Gemini API` `LangSmith`

**Vision**
`OpenCV` `PIL` 

**General**
`Python` `Git` `Jupyter` `Google Colab` `macOS (Apple Silicon)`

---

### Projects

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

### Certifications

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

**IBM SkillsBuild**

[![Agentic AI with LangChain & LangGraph](https://img.shields.io/badge/Agentic%20AI%20%7C%20LangChain%20%26%20LangGraph-IBM%20SkillsBuild-054ADA?style=flat-square&logo=ibm&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Agentic%20AI%20with%20LangChain%20and%20LangGraph.pdf)

**DeepLearning.ai**

[![Retrieval Augmented Generation](https://img.shields.io/badge/Retrieval%20Augmented%20Generation-DeepLearning.ai-0B6E4F?style=flat-square&logo=coursera&logoColor=white)](https://github.com/taeyang0505/taeyang0505/blob/main/Retrieval%20Augmented%20Generation.png)

---

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/HuggingFace-FFD21F?style=flat-square&logo=huggingface&logoColor=black"/>
</p>
