Final project

# Emotion Detection Application

This project is a web-based Emotion Detection application built using Flask and IBM Watson NLP. The application analyzes user-provided text and returns emotion scores along with the dominant emotion.

## Project Overview

The application performs the following tasks:

- Sends user input text to the Watson NLP EmotionPredict API
- Extracts emotion scores (anger, disgust, fear, joy, sadness)
- Determines the dominant emotion
- Displays results through a Flask web interface
- Includes unit testing for validation
- Implements error handling for invalid input
- Passes static code analysis using pylint

## Technologies Used

- Python 3
- Flask
- Requests library
- IBM Watson NLP API
- unittest (for unit testing)
- pylint (for static code analysis)

## Project Structure

final_project/
│
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
│
├── templates/
│   └── index.html
│
├── static/
│   └── mywebscript.js
│
├── test_emotion_detection.py
├── server.py
└── README.md

## How to Run the Application

1. Navigate to the project folder:
   python3 server.py

2. Open your browser and visit:
   http://localhost:5000

3. Enter text to analyze emotions.

## Example Output

For input:
I love my life

Output:
For the given statement, the system response is 'anger': 0.006274985, 'disgust': 0.0025598293, 'fear': 0.009251528, 'joy': 0.9680386 and 'sadness': 0.049744144. The dominant emotion is joy.

## Error Handling

If the user submits blank input, the application returns:

Invalid text! Please try again!

## Unit Testing

To run unit tests:
python3 test_emotion_detection.py

All tests must pass successfully.

## Static Code Analysis

Run:
pylint server.py

Target score:
10.00/10