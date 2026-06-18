## Hi, I'm Taeyang 👋

I'm an AI Engineering student at Inha University with a strong interest in **Computer Vision** and **Multimodal AI**. I've spent the last year digging into Vision-Language Models (VLMs) as an undergraduate research assistant — specifically on the problem of object hallucination, where models confidently describe things that aren't in the image.

Beyond research, I like building things that actually run. Most of my recent projects sit at the intersection of LLMs, RAG pipelines, and practical deployment.

---

### What I'm working on

- Finishing up **RoboGuard**, an RLAIF-based RAG agent for industrial robot manuals that uses a self-correction loop (LangGraph + Gemini) to catch and fix hallucinated responses before they reach the user
- Exploring how inference-time defense strategies (like **B-VCD**) can make VLMs more reliable without any retraining

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
Training-free hallucination defense for VLMs at inference time. Adds realistic sensor noise (motion blur + Poisson-Gaussian) to perturb visual input and uses contrastive decoding to suppress hallucinated tokens. Evaluated with an automated LLM-as-a-Judge pipeline.

**[Emotion-Aware Multimodal Chatbot](https://github.com/taeyang0505/Emotion_Aware_Multimodal_Chatbot_Project_Text_Image_and_Response_Generation)**
Combines BiLSTM + Attention for text emotion recognition with EfficientNet for image emotion, then fuses both modalities to generate context-aware responses.

**[Pneumonia Classification](https://github.com/taeyang0505/Pneumonia-Classification-Project)**
CNN-based chest X-ray classifier built with TensorFlow/Keras.

**[Forest Cover Classification](https://github.com/taeyang0505/Forest_Cover_Classification_Project)**
Multi-class tabular classification using tree-based and ensemble methods.

---

### Certifications

Naver Boostcourse — AI Basics (×2), CV, DL, NLP, Linear Algebra, Model Compression  
Codecademy — LangChain & LangGraph, RAG, NLP, LLMs, ML/AI Engineer Path, DL with TensorFlow

---

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/HuggingFace-FFD21F?style=flat-square&logo=huggingface&logoColor=black"/>
</p>
