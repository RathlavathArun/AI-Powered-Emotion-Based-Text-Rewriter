# AI-Powered-Emotion-Based-Text-Rewriter

# ✍️ EmotionScribe: AI-Powered Emotion-Based Text Rewriter

EmotionScribe is a **Streamlit web app** that rewrites your text according to your **facial emotion**.  
It uses **DeepFace** to detect your mood from a photo or webcam, and then calls a **local Ollama model (LLaMA 3)** to produce **emotionally aligned text rewrites** — or intelligent fallbacks when offline.

---

## 🚀 Features

✅ **Real-Time Emotion Detection**
- Detects emotions using **DeepFace** (OpenCV backend).  
- Automatically filters out “neutral” responses and selects the next most expressive emotion.  

✅ **AI-Based Text Rewriting**
- Uses **Ollama’s LLaMA 3** local model to rewrite text in the tone of the detected emotion.  
- Each output generates **3 contextual synonyms** with matching emotional tone.

✅ **Fallback System**
- If Ollama is unavailable, it switches to **contextual fallback templates** (happy, angry, sad, etc.) so users still get emotion-based rewrites.

✅ **Cyber Dark UI Theme**
- Futuristic dark layout with glowing buttons, badges, and emotion cards.  
- Separate sections for input, camera capture, and rewrites.

✅ **Image or Camera Input**
- Upload an image or take a live camera snapshot to detect your current mood.

---

## 🧠 How It Works

1. Enter a text you want rewritten.  
2. Capture or upload your face image.  
3. DeepFace detects your dominant emotion (excluding neutral).  
4. Ollama (LLaMA 3 model) rewrites your text to match the detected tone.  
5. View and cycle through **3 different emotionally-tuned rewrites**.

---

## 🧰 Tech Stack

| Component | Purpose |
|------------|----------|
| **Streamlit** | Web Interface |
| **DeepFace** | Emotion Detection |
| **Ollama (LLaMA 3)** | Local Text Rewriting |
| **OpenCV** | Face Recognition Backend |
| **Pillow (PIL)** | Image Handling |
| **NumPy** | Array Processing |
| **Requests** | Ollama API Calls |

---

## ⚙️ Installation dependencies
pip install streamlit deepface opencv-python pillow numpy requests

## Run Ollama (if using local model)
Make sure Ollama is installed and the LLaMA 3 model is pulled:

ollama pull llama3:8b
ollama run llama3:8b
TO run it:
streamlit run filename.py

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/RathlavathArun/AI-Powered-Emotion-Based-Text-Rewriter.git
cd EmotionScribe




