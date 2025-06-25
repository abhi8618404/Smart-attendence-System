# 🎓 Smart Attendance System (Face Recognition)

A real-time **Face Recognition-based Attendance System** developed in **Python**, **OpenCV**, and **Tkinter GUI**. This project automates attendance marking by capturing faces via webcam, recognizing users based on a trained model, and logging attendance in `.csv` files.

[![Made with Python](https://img.shields.io/badge/Made%20with-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
[![OpenCV](https://img.shields.io/badge/Library-OpenCV-red?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)

---

## 🚀 Features

- 📷 Register new users by capturing facial images  
- 🧠 Train face recognition model (LBPH algorithm)  
- 🤖 Recognize faces from webcam feed  
- 🗓️ Auto-log attendance with timestamp  
- 📂 Save attendance in `Attendance_<subject>_<date>.csv`  
- 📊 View attendance records through GUI

---

## 🔧 Setup & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/abhi8618404/Smart-attendence-System.git
   cd Smart-attendence-System
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Create storage folder

bash
Copy
Edit
mkdir TrainingImage
Adjust file paths

Open .py files (e.g. attendance.py, automaticAttendance.py), update any local paths to match your environment.

Start the application

bash
Copy
Edit
python attendance.py
💡 How It Works
The system follows this simple flow:

Register User

Enter ID & name → webcam captures ~50 face images

Images are stored in TrainingImage/ID_Name/

Train Model

Encode stored images → generate face recognition model

Model saved as Trainer.yml

Mark Attendance

Run automaticAttendance.py → enter subject name

Real-time face recognition logs attendance to Attendance_<subject>_<date>.csv

View Records

Use GUI to select and display any .csv attendance file

📁 Directory Structure
bash
Copy
Edit
Smart-attendence-System/
├── attendance.py              # GUI & registration logic
├── automaticAttendance.py    # Real-time attendance capture
├── trainImages.py            # Train face recognition model
├── TrainingImage/            # Captured user faces
├── requirements.txt
└── README.md
📸 Sample Screenshots
(Replace these with your own images)

Main GUI

Registering a user

Live attendance being recorded

Viewing attendance CSV

📦 Tech Stack
Python 3

OpenCV – for face detection + recognition (LBPH)

Tkinter – GUI interface

NumPy / Pandas – image processing & CSV handling

🔮 Future Improvements
Migrate from CSV to SQLite/MySQL

Add user authentication (admin vs student login)

Export attendance data as PDF

Enhance recognition accuracy with deep learning models
