# 🌿 AgroLens - AI-Based Plant Disease Detection System

AgroLens is a smart and intuitive web application that uses artificial intelligence to detect plant diseases from leaf images. It empowers farmers, gardeners, and agricultural experts with quick and reliable diagnostics to support healthier crops and improve agricultural productivity.

## 🚀 Features

- 🔍 **Plant Disease Detection** – Upload a leaf image and get instant results on the disease type (if any).
- 🧠 **AI-Powered Model** – Utilizes a trained deep learning model for accurate classification.
- 📸 **Image Upload Interface** – Clean and user-friendly UI to upload and analyze images.
- 📊 **Result Dashboard** – Displays disease information, confidence score, and suggestions.
- 🪴 **Support for Multiple Crops** – Trained on a variety of plant species (e.g., tomato, potato, maize, etc.).

## 🛠️ Tech Stack

- **Frontend**: Html, CSS, React.js
- **Backend**: Node.js
- **Database**: MongoDB
- **Machine Learning**: Python (Flask-based)
- **Deployment**: Localhost

## 🖼️ System Architecture

AgroLens follows a decoupled architecture, enabling smooth communication between the frontend, backend, and AI services.

![AgroLens Architecture Diagram](./assets/architecture.png)

**Component Flow:**

1. **React Frontend**  
   → Collects and uploads leaf images .
2. **Node.js Backend (No Express)**  
   → Receives image data and routes it to the Python-based AI model using HTTP requests .

3. **Flask AI Model Server**  
   → Processes the image, runs the AI model, and returns prediction results (disease name + confidence).

4. **MongoDB Database** *(optional)*  
   → Stores logs, reports, or user data (can be skipped for MVP).

5. **Frontend**  
   → Displays results with recommendations and an interactive UI.


### Clone and Set Up

```bash
git clone https://github.com/yourusername/AgroLens.git
cd AgroLens
