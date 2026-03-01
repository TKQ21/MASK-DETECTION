# 😷 Face Mask Detection System (Real-World Ready)

A production-grade **Face Mask Detection Web Application** that detects whether a person is **wearing a mask properly, not wearing a mask, or wearing it incorrectly** using real-time camera feed or image upload.

PROJECT:https://mask-detection.lovable.app

---

## 🚀 Features

- ✅ Real-time face mask detection using webcam
- 📷 Image upload based detection
- 🟢 Mask / 🔴 No Mask / 🟡 Incorrect Mask classification
- 📦 Handles real-world conditions:
  - Low light
  - Multiple faces
  - Side faces & tilted angles
  - Glasses, beard, different mask colors
- 📊 Confidence score & bounding box visualization
- ⚠️ User-friendly error handling
- 📱 Mobile & desktop responsive UI

---

## 🧠 Tech Stack

### Frontend
- React.js / Next.js
- Tailwind CSS
- Webcam API
- Axios

### Backend
- Python
- FastAPI
- OpenCV
- YOLO / MobileNet based CNN model
- ONNX / Torch optimized inference

---

## 🏗️ Project Structure
mask-detection-system/
│
├── backend/
│ ├── main.py
│ ├── detector.py
│ ├── model/
│ ├── logs/
│ └── requirements.txt
│
├── frontend/
│ ├── components/
│ ├── pages/
│ ├── hooks/
│ └── services/api.js
│
├── docker-compose.yml
└── README.md


---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|------|---------|-------------|
| POST | /detect-image | Detect mask from uploaded image |
| POST | /detect-frame | Detect mask from video frame |
| GET | /health | Backend health check |
| GET | /model-info | Model details |

---

## ⚠️ Error Handling

- No face detected
- Multiple faces detected
- Camera access denied
- Invalid image format
- Low confidence detection
- Backend unavailable

---

## 🧪 Detection Labels

- **Mask**
- **No Mask**
- **Mask Worn Incorrectly**

If confidence < 60%, result shows:
> "Unable to determine mask status clearly"

---

## 🐳 Deployment

- Docker-ready backend
- Environment variable support
- CPU & GPU compatible
- Scalable architecture

---

## 🛠️ Setup Instructions

### Backend
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
Frontend
cd frontend
npm install
npm run dev
🎯 Use Cases

Schools & Colleges

Offices

Hospitals

Public Places

Entry Gate Monitoring

📌 Future Enhancements

Admin dashboard

Violation counter

CSV export

CCTV stream support

👨‍💻 Author
MOHD KAIF
DATA SCIENCE | DATA ANALYST | GEN AI
