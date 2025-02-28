# Attendence-by-Face-Recognition
Attendance by Face Recognition

Project Overview

This project implements an automated Attendance System using Face Recognition Technology. The system leverages Python, OpenCV, Pandas, Numpy, and Streamlit to capture images of individuals through a webcam, recognize their faces, and mark attendance accordingly. The attendance data is stored in a CSV file, enabling easy tracking and management of students or employees. Streamlit is used for building a simple web-based interface for real-time interaction.

Key Features

Face Recognition: Utilizes OpenCV and pre-trained models to detect and recognize faces.
Automatic Attendance Logging: Captures the time of recognition and stores it in a CSV file (Pandas).
Real-time Display: A web-based user interface built with Streamlit, displaying live webcam feed and attendance logs.
CSV Data Storage: Attendance details, such as name and time of entry, are saved into a CSV file using Pandas for easy access and manipulation.
Technologies Used

Python: Main programming language.
OpenCV: Used for real-time face detection and recognition.
Pandas: Used for managing and storing attendance data in a CSV format.
Numpy: Used for numerical operations and image array manipulation.
Streamlit: Provides an interactive web interface to display the webcam feed and attendance details.
Installation

To run this project locally, you need to install the required dependencies. Follow these steps:

Clone the repository:

Bash

git clone https://github.com/majumdarjoyeeta/Attendance-by-Face-Recognition.git
cd Attendance-by-Face-Recognition
Install the necessary libraries:

Bash

pip install -r requirements.txt
Run the Streamlit application:

Bash

streamlit run app.py
Access the interface through your browser at http://localhost:8501.

How it Works

Face Detection: When the app is launched, it accesses your webcam feed. Using OpenCV, the system detects faces in real time.
Face Recognition: The system recognizes the faces of enrolled individuals and matches them with stored data (e.g., name).
Attendance Logging: Once a face is recognized, the system logs the time and the person's name in the attendance CSV file.
Streamlit Interface: The live webcam feed is shown on the web interface, and the attendance data can be viewed in real-time.
How to Use

Enrollment: Initially, you need to capture images of all individuals whose attendance will be tracked. This can be done using a simple function to add a name and corresponding face images to the system.
Take Attendance: Once enrolled, launch the app, and the system will continuously monitor for faces. When it recognizes a face, it will automatically mark the person’s attendance.
View Attendance: The attendance record (including the date and time) can be viewed and exported from the CSV file.
Folder Structure

Attendance-by-Face-Recognition/
├── Attendance/
│   ├── Attendance_28-02-2025.csv
├── data/
│   ├── faces_data.pkl
│   ├── haarcascade_frontalface_default.xml
│   └── names.pkl
├── add_faces.py
├── app.py
├── background.png
├── README.md
└── test.py
Future Enhancements

Add a feature to automatically send attendance data to an admin or teacher via email.
Integrate with existing database systems like MySQL or SQLite for large-scale deployment.
Improve face recognition accuracy using deep learning models.
Implement real-time notifications for successful or failed face recognition.
