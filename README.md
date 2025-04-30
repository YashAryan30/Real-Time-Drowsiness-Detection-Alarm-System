# Real-Time-Drowsiness-Detection-Alarm-System

This project is a real-time driver drowsiness detection system using OpenCV, MediaPipe, and Twilio. It detects early signs of fatigue based on eye aspect ratio (EAR) and triggers an alarm, sends an SMS, and initiates a phone call with GPS location if drowsiness is sustained.

📌 Features
🔍 Real-time facial landmark detection using MediaPipe
👁️ Calculates EAR to detect drowsiness
⏱️ Triggers alarm only after 3 seconds of sustained drowsiness
📱 Sends an SMS alert with location link
📞 Initiates an emergency call via Twilio
🗺️ Logs drowsiness events with timestamp and coordinates
🧠 Multithreaded alerts for smooth performance

🛠️ Tech Stack
Python 3
OpenCV
MediaPipe
NumPy
Twilio API
Geocoder
Pygame
CSV Logging

🧠 How It Works
Captures webcam feed and detects facial landmarks using MediaPipe.
Calculates EAR from eye landmarks.
If EAR < 0.25 for more than 3 seconds:
Plays an alarm sound.
Sends an SMS with time, location, and a map link.
Initiates a phone call using Twilio.
Logs the event into a CSV file.

📝 Future Improvements
Add GUI dashboard
Integrate email alerts
Store logs in a database
Add Yawn detection and head tilt detection
