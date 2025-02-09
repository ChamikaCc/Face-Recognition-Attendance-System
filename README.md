# Face Recognition Attendance System

## Project Overview

The Face Recognition Attendance System is an automated solution for tracking student attendance using facial recognition technology. The system captures, processes, and identifies student faces through a webcam and records their attendance in a structured format. This eliminates the need for manual attendance marking, reducing errors and saving time.

## Key Features

Face Detection & Recognition: Uses OpenCV’s Haar Cascade Classifier to detect faces and a machine learning model (K-Nearest Neighbors) to recognize individuals.
Automated Attendance Recording: Recognized faces are logged into a CSV file with the student’s name, ID, and timestamp.
User Registration: New users can add their face data, and the system will train the recognition model accordingly.
Real-time Processing: The system captures live video from the webcam, detects faces, and updates the attendance in real-time.
Flask Web Interface: Users can access attendance records through a web-based interface.
Data Persistence: Attendance records are stored in CSV format, and trained models are saved for future recognition.

## Technical Stack
+ Python (Primary language)
+ Flask (Web framework)
+ OpenCV (Face detection)
+ scikit-learn (Machine learning for face recognition)
+ Joblib (Model serialization)
+ Pandas (Data handling)
+ Waitress (Production server)

## How It Works
User Registration: A student registers by providing their name and student ID. The system captures multiple images of their face.
Training the Model: The system extracts features from the collected images and trains a K-Nearest Neighbors (KNN) model.
Attendance Marking: When a student appears in front of the camera, their face is detected, identified, and logged into the attendance file.
Attendance Viewing: The recorded attendance can be viewed via a web interface.
