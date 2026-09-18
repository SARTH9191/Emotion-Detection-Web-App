# Emotion Detection Web Application

An AI-powered web application that detects and analyzes emotions from textual statements using the Watson NLP EmotionPredict service and a Flask backend.

## Project Description

The Emotion Detector application evaluates text statements and provides confidence scores across five primary emotional categories:
- **Anger**
- **Disgust**
- **Fear**
- **Joy**
- **Sadness**

It also evaluates and displays the **dominant emotion** with the highest score. If an invalid or empty text string is submitted, robust error handling returns a user-friendly error notification.

---

## Directory Structure

```text
final_project/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   ├── mywebscript.js
│   └── style.css
├── templates/
│   └── index.html
├── README.md
├── requirements.txt
├── server.py
└── test_emotion_detection.py
```

---

## Installation & Setup Instructions

### 1. Clone or Navigate to the Repository
```bash
cd final_project
```

### 2. Install Required Dependencies
Ensure Python 3.8+ and pip are installed, then install the dependencies:
```bash
pip install flask requests pylint
```

### 3. Run Unit Tests
Validate the emotion detector against standard benchmark sentences:
```bash
python3 -m unittest test_emotion_detection.py
```

### 4. Check Code Quality with Pylint
Ensure the Flask application adheres strictly to PEP 8 standards:
```bash
pylint server.py
```

### 5. Launch the Web Application
Start the Flask development server on port 5000:
```bash
python3 server.py
```

Open your browser and navigate to:
```
http://localhost:5000
```
