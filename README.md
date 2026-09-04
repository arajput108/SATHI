# SĀTHI — Smart Adaptive Tutor and Human Interaction

SĀTHI stands for **Smart Adaptive Tutor and Human Interaction**.

SĀTHI is an AI-powered practice and learning companion developed as a prototype for **Smart India Hackathon 2026** under the **Smart Automation — Software** category.

The idea behind SĀTHI is simple: instead of only showing a person how something is done, the system observes their practice, evaluates their performance, and provides feedback to help them improve.

The current prototype demonstrates this idea through **real-time exercise form analysis using a camera**.

---

## What SĀTHI Does

The current prototype allows a user to:

- Start their camera and track body movement
- Practice a squat exercise
- Detect body pose using MediaPipe
- Measure knee and back angles
- Count completed repetitions
- Detect full-depth repetitions
- Track exercise tempo and movement phase
- Calculate a session score out of 100
- View session time and performance statistics
- Receive live coaching feedback
- Run a demonstration without using a camera

The prototype is intentionally focused on one exercise so that the core concept can be demonstrated clearly.

---

## How It Works

SĀTHI follows a simple practice and feedback cycle:

1. The user chooses an activity or skill.
2. The system observes the user's practice.
3. Computer vision models analyze the user's movements.
4. The system evaluates the performance.
5. Feedback is provided to the user.
6. The user's performance can be used to improve future practice sessions.

In the current prototype, this workflow is demonstrated using a squat exercise.

The application uses body landmarks detected through **MediaPipe Pose Landmarker** to estimate movement and calculate different performance metrics.

---

## Current Prototype

The current version is a browser-based prototype contained in a single HTML file.

It includes:

- Real-time camera input
- Pose landmark detection
- Squat repetition counting
- Knee-angle analysis
- Back-angle analysis
- Movement phase detection
- Tempo tracking
- Full-depth repetition tracking
- Live form scoring
- Coaching feedback
- Session statistics
- No-camera demonstration mode

The prototype performs the core analysis locally in the browser.

---

## Technologies Used

### Current Prototype

- HTML5
- CSS3
- JavaScript
- MediaPipe Pose Landmarker
- HTML Canvas
- Web Camera API

### Proposed Full System

The complete SĀTHI architecture is designed around:

- **Flutter (Dart)** — Application development
- **FastAPI (Python)** — Backend services
- **PostgreSQL** — Persistent data storage
- **Redis** — Live session state
- **OpenCV** — Computer vision processing
- **MediaPipe** — Pose and gesture analysis
- **AI models** — Feedback and personalization
- **Gemini API** — Planned multimodal reasoning layer

---

## Project Structure

```text
SATHI/
└── index.html
