# Hand Sign Classification — A to Y

A multi-class CNN image classifier built from scratch in PyTorch that recognizes **24 American Sign Language (ASL) hand sign alphabets** (A–Y, excluding J which requires motion).

---

## Demo

Live inference runs directly from your webcam using OpenCV.

---

## Model Weights

> ⚠️ The `.pth` file (~100MB) is **not tracked in this repo**. Download it from Releases.

**[⬇ Download model weights (v1.0)](https://github.com/Deep-ii/Hand_Sign-Classification/releases/tag/v1.0)**

---

## Project Structure

```
Hand_Sign-Classification/
│
├── Handsign_project.ipynb   # Full pipeline: training, evaluation, live inference
└── README.md
```

---

## Pipeline Overview

```
Raw Images (24 classes)
        ↓
Preprocessing (Resize, Normalize)
        ↓
CNN Model (Conv → Pool → FC layers)
        ↓
Softmax Output (A–Y)
        ↓
Live Webcam Inference (OpenCV)
```

---

## Classes

24 static hand signs — **A through Y**, skipping J (requires motion).

---

## Setup & Usage

### 1. Clone the repo

```bash
git clone https://github.com/Deep-ii/Hand_Sign-Classification.git
cd Hand_Sign-Classification
```

### 2. Install dependencies

```bash
pip install torch torchvision opencv-python
```

### 3. Download the model

Download `handsign_model.pth` from **[Releases](https://github.com/Deep-ii/Hand_Sign-Classification/releases/tag/v1.0)** and place it in the project root.

### 4. Run inference

Open `Handsign_project.ipynb` and run the **Live Inference** section. It will open your webcam and start predicting in real time.

---

## Tech Stack

| Component | Tool |
|-----------|------|
| Framework | PyTorch |
| Architecture | Custom CNN |
| Live Inference | OpenCV |
| Notebook | Jupyter |

---

## What I Learned

- Designing a CNN architecture from scratch (Conv, Pool, FC layers)
- Debugging shape and device mismatches in PyTorch
- Saving and loading model weights with `torch.save` / `torch.load`
- Running live webcam inference with OpenCV

---

## Author

**Deep** — [GitHub](https://github.com/Deep-ii)
