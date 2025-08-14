# 🎓 Smart Attendance System (Face Recognition)

A **real-time Face Recognition-based Attendance System** developed in **Python**, **OpenCV**, and **Tkinter GUI**.  
This project automates attendance marking by capturing faces via webcam, recognizing users based on a trained model, and logging attendance in `.csv` files.

[![Made with Python](https://img.shields.io/badge/Made%20with-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
[![OpenCV](https://img.shields.io/badge/Library-OpenCV-red?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)

---

## 🚀 Features

- 📷 Register new users by capturing facial images.  
- 🧠 Train face recognition model (**LBPH algorithm**).  
- 🤖 Recognize faces from webcam feed in real time.  
- 🗓️ Auto-log attendance with timestamps.  
- 📂 Save attendance in `Attendance_<subject>_<date>.csv`.  
- 📊 View attendance records via GUI.

---

## 🔧 Setup & Usage

### 1️⃣ Clone the repository
```bash
git clone https://github.com/abhi8618404/Smart-attendence-System.git
cd Smart-attendence-System
```

### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Create storage folder
```bash
mkdir TrainingImage
```

### 4️⃣ Adjust file paths
Open `.py` files (e.g., `attendance.py`, `automaticAttendance.py`) and update any local paths to match your environment.

### 5️⃣ Start the application
```bash
python attendance.py
```

---

## 💡 How It Works

1. **Register User**  
   - Enter ID & Name → Webcam captures ~50 face images.  
   - Images stored in `TrainingImage/ID_Name/`.

2. **Train Model**  
   - Encodes stored images → Generates recognition model.  
   - Model saved as `Trainer.yml`.

3. **Mark Attendance**  
   - Run `automaticAttendance.py` → Enter subject name.  
   - Recognized faces logged in `Attendance_<subject>_<date>.csv`.

4. **View Records**  
   - Use GUI to select & display any `.csv` attendance file.

---

## 📁 Directory Structure
```
Smart-attendence-System/
├── attendance.py            # GUI & registration logic
├── automaticAttendance.py   # Real-time attendance capture
├── trainImages.py           # Train face recognition model
├── TrainingImage/           # Captured user faces
├── requirements.txt
└── README.md
```

---

## 📸 Sample Screenshots
*(Replace with your own images)*  
- Main GUI  
- Registering a user  
- Live attendance being recorded  
- Viewing attendance CSV  

---

## 📦 Tech Stack

- **Python 3**  
- **OpenCV** – Face detection & recognition (LBPH)  
- **Tkinter** – GUI interface  
- **NumPy / Pandas** – Image processing & CSV handling  

---

## 🔮 Future Improvements

- Switch from CSV to **SQLite/MySQL** for better storage.  
- Add **user authentication** (admin vs student login).  
- Export attendance data as **PDF**.  
- Improve accuracy with **deep learning models**.
