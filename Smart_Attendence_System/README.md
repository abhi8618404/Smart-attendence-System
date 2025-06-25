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
