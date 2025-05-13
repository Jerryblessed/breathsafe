
# 🫁 Breath Safe

[Presentation](https://docs.google.com/presentation/d/1r_a98Et5a3CCOZtHDk0O5rNGh_tOkeDCvzrJvdH8OQA/edit?usp=sharing)
🔗 **View the project pitch deck**

![Breath Safe Landing Page](https://github.com/Jerryblessed/breathsafe/blob/main/static/landingpage.png?raw=true)

**Breath Safe** is a lightweight Flask application that democratizes AI-powered lung cancer diagnosis using both deep learning and no-code tools. Built for low-resource settings, the platform enables non-technical health workers to upload CT or histopathology images via a simple web UI for instant predictions and guidance.

---

## 🚀 Features

* 🖼️ **Dual Image Upload**
  - Supports both CT and histopathology images.
  - Upload via drag-and-drop interface on the web app.
* 🧠 **High-Fidelity Deep Learning**
  - Backend runs a DenseNet121 model trained on **16,000+ images** for accurate, offline-ready inference.
* 💡 **No-Code Azure Option**
  - For clinics with limited technical capacity, 800 pre-labeled lung images were trained on **Azure Custom Vision** for an easy plug-and-play interface.
* 🤖 **AI Chatbot Assistant**
  - Integrated with Azure OpenAI to explain results, answer lung-health questions, and guide users through uploads.
* 🔐 **Secure Viewer Access**
  - Azure Custom Vision access managed via viewer lists—no exposed secrets.

---

## 🎯 Uniqueness

1. **Dual Training Paths**
   - A powerful deep learning model (DenseNet121) trained locally on 16K lung images.
   - A parallel no-code model trained on 800 curated samples using Azure Custom Vision for accessible cloud-based use.
2. **Two Modalities, One Platform**
   - Handles both CT scans and histopathology slides with equal ease.
3. **Offline-Ready Architecture**
   - Local model designed for containerized inference in remote clinics.
4. **Embedded AI Agent**
   - Helps interpret model outputs and provides clinical context in plain English.

---

## 🌍 Social Good

* **Bridging diagnostic gaps** in rural clinics (currently <15% imaging coverage).
* **Advancing SDG 3.4**: Early detection could help save over 600,000 lives annually.
* **Empowering non-specialists**: AI helps community health workers participate in diagnosis and triage.
* **Fostering collaboration**: Viewer access and open-source codebase encourage transparency and feedback.

---

## 🛠️ Getting Started step 1: Download models from drive
[download models here](https://drive.google.com/drive/folders/17am-HyZ2R7SoCi9Rpfu5uK71XAWWI1ff?usp=drive_link)
🔗 **Model download**
```bash
# place both models in root directory of flask app
````

## 🛠️ Getting Started step 2: install files

```bash
# Clone the repo
git clone https://github.com/Jerryblessed/breathsafe.git
cd breathsafe

# Create virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install flask requests azure-ai-vision openai

# Run the app
python app.py
````

Visit `http://localhost:5000` in your browser to explore.

---

© 2025 Breath Safe Initiative

