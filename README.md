# Attendance-Monitoring-via-Face-recognition

🚀 How It Works
1️⃣ Face Enrollment

New faces are registered using facetrain.py.

The script captures facial images, extracts key features, and saves the data for recognition.

---

2️⃣ Face Recognition

recognizer.py performs real-time face recognition using the Local Binary Pattern Histogram (LBPH) algorithm.

When a stored face is matched, the model retrieves the associated student/user information.

---

3️⃣ Attendance Logging

Recognized individuals are automatically marked as Present in a CSV log.

Each entry includes:

Name

Time stamp

Date

Recognition result

---

🧠 Technology Used

Python

OpenCV

NumPy

CSV for attendance logging

LBPH (Local Binary Pattern Histogram) for robust face recognition

---

⭐ Highlights

Fully automated attendance marking

Works in real-time via webcam

Uses classical computer vision — no heavy GPU required

Easy to extend into an admin dashboard or API

---

⚠️ Note on Accuracy

Recognition results heavily depend on:

Webcam quality

Lighting conditions

Variation in the training images

Capturing well-lit, front-facing training images significantly improves performance.

---

📂 Folder Structure 


.
├── facetrain.py
├── recognizer.py
├── Attendance.csv
├── /dataset
└── README.md

---
🔧 Future Enhancements 

Add a GUI dashboard for admin operations

Replace LBPH with a deep learning model (e.g., FaceNet / Dlib embeddings)

Add attendance insights & graphs

Integrate with a cloud database

