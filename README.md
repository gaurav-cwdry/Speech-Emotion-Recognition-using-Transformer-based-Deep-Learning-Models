# Speech Emotion Recognition using Transformer-based Deep Learning Models

### B.Tech Third Year Project

**Title:** Speech Emotion Recognition using Transformer-based Deep Learning Models  
**Student Name:** Gourab Chowdhury  
**Roll Number:** 22CS3069  
**Supervisor:** Dr. Susham Biswas  
**Department:** Computer Science and Engineering  
**Semester:** 6th

---

## 📌 Introduction

Speech Emotion Recognition (SER) is a growing field at the intersection of speech processing and affective computing. It enables machines to detect the emotional state of a speaker using vocal cues.  
This project proposes a deep learning-based approach using the pre-trained transformer model **Wav2Vec2** to identify emotions such as happiness, sadness, anger, and neutrality directly from raw audio.

---

## 🎯 Objectives

- Build a robust model to classify emotions from speech.  
- Use pre-trained audio language models like **Wav2Vec2** for feature extraction.  
- Fine-tune the model on labeled emotion datasets.  
- Prepare for future deployment in real-time applications.

---

## 📂 Dataset Description

The dataset used was sourced from **Kaggle**, consisting of `.wav` audio files labeled with seven basic emotions:

- Angry  
- Happy  
- Sad  
- Neutral  
- Fear  
- Disgust  
- Surprise

Each file is labeled via its filename and is sampled at a consistent rate suitable for deep learning models.

---

## 🧠 Methodology

### 🔹 Data Preprocessing
- Loaded `.wav` files using **Librosa** and **Torchaudio**  
- Cleaned and structured labels using **Pandas DataFrame**  
- Visualized waveforms and spectrograms for pattern analysis

### 🔹 Feature Extraction
- Used **Wav2Vec2Processor** from HuggingFace to tokenize audio  
- Extracted embeddings using **Wav2Vec2ForSequenceClassification**

### 🔹 Model Training
- Built a custom **PyTorch Dataset** class  
- Used **HuggingFace’s Trainer API** for model training  
- Optimized using **Cross-Entropy Loss**  
- Evaluated using **Accuracy Score**

---

## ✅ Results

- The model showed promising performance in identifying different emotions  
- Frequently occurring emotions like **happy**, **sad**, and **angry** were well-classified  
- **Confusion Matrix** and **Accuracy Score** indicated effective learning  

> 📌 *Actual metrics and visualizations will be added after full training*

---

## 🛠️ Technologies Used

- Python (Google Colab)  
- PyTorch & HuggingFace Transformers  
- Librosa & Torchaudio  
- Pandas, Matplotlib, Seaborn

---

## ⚠️ Challenges Faced

- Class imbalance in the dataset  
- Variability in speaker accent and volume  
- GPU limitations while training large models

---

## 🚀 Future Scope and Extensions

### 🔹 Real-Time User Interface Development
- A web-based interface using **Streamlit** or **Gradio** for real-time emotion prediction  
- Users can record voice and get instant emotion feedback

### 🔹 Multimodal Emotion Recognition
- Combine facial expressions using **VGGFace** or **OpenFace** along with speech

### 🔹 Data Augmentation and Expansion
- Use external datasets like **RAVDESS**, **CREMA-D**, **TESS**  
- Apply augmentations like **noise addition**, **pitch shifting**, etc. using `audiomentations`

### 🔹 Model Improvement
- Explore models like **HuBERT**, **Whisper**, **XLS-R**  
- Combine with sequential layers like **LSTM/GRU**

### 🔹 Emotion Analytics Dashboard
- Visual dashboard showing emotion trends, pitch-energy analysis, and user history

### 🔹 Explainability
- Use tools like **SHAP** or **LIME** for interpreting predictions  
- Show **attention maps** over audio signals

---

## 🏁 Conclusion

This mid-term progress report demonstrates successful implementation of a **transformer-based speech emotion recognition** system. The results are promising, and with the planned extensions, this project has the potential to evolve into a real-time SER system for applications in **healthcare**, **virtual assistants**, and **customer service**.

---

