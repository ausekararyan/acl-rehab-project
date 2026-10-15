# RePitch - ACL Rehabilitation Interactive Portal

An interactive, AI-assisted ACL Rehabilitation Portal designed for guided patient recovery and automated physiotherapist telemetry.

---

## 🚀 Overview

This repository contains the standalone **Interactive Prototype / Portal** (`acl-rehab-portal.html` / `index.html`) featuring:
- **Patient Dashboard & Guided Exercise Sets**: 1 Set, 1 Rep recovery protocol with real-time pose guidance and audio cues.
- **Computer Vision Posture Tracking**: Uses MediaPipe Pose engine for joint angle tracking (knee extension, hip flexion) directly in the browser via webcam.
- **Smart Video Highlight Clipper**: Synchronized 10-second highlight reel demonstrating all 4 Phase 1 recovery exercises (Quad Sets, SLR, Heel Slides, Patellar Mobilizations).
- **Autonomous Agentic Physio Workflow**: Automatically packages exercise telemetry, extension lag, accuracy, and video timestamps into structured clinical reports dispatched directly to the clinician dashboard.
- **Physiotherapist Dashboard**: Real-time review feed, compliance scoring, pain tracking, ROM (Range of Motion) metrics, and automated triage ticket generation.

---

## 📁 Repository Structure

```text
acl-rehab-project/
├── index.html                           # Main entrypoint (GitHub Pages ready)
├── acl-rehab-portal.html                # Interactive portal prototype
├── phase_1_combined.mp4                 # 10-second highlight video of Phase 1 exercises
├── exercise_quad_sets_1787543982867.jpg # Exercise reference: Quad Sets
├── exercise_slr_1787543996071.jpg       # Exercise reference: Straight Leg Raise
├── exercise_heel_slides_1787544005962.jpg # Exercise reference: Heel Slides
├── exercise_knee_mob_1787544028496.jpg  # Exercise reference: Patellar Mobilizations
├── logo_transparent.png                 # RePitch branding logo
├── .user_uploaded/
│   └── media_1787583769820.png          # Roo Mascot avatar
└── README.md
```

---

## 💻 How to Run Locally

### Option 1: Direct File
Simply open `index.html` or `acl-rehab-portal.html` in any modern web browser (Google Chrome or Microsoft Edge recommended for webcam/MediaPipe features).

### Option 2: Local HTTP Server (Recommended)
Run Python's built-in web server:

```bash
# From within the repository directory
python3 -m http.server 8080
```

Then visit:
- **[http://localhost:8080](http://localhost:8080)** or **[http://localhost:8080/acl-rehab-portal.html](http://localhost:8080/acl-rehab-portal.html)**

---

## 🌐 Deploy to GitHub Pages

1. In GitHub, go to your repository **Settings** -> **Pages**.
2. Under **Build and deployment**, set the source to `Deploy from a branch`.
3. Select the `main` branch and `/ (root)` folder.
4. Click **Save**. Your portal will be live on the web!
