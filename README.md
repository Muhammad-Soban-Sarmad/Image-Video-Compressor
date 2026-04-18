# 🗜️ MediaCrush — Image & Video Compressor

A fast, local, browser-based media compressor built with Streamlit.  
Compress images and videos without uploading anything to a server — everything runs on your machine.

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.x-red?style=flat-square&logo=streamlit)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## ✨ Features

- **Image compression** — JPEG, PNG, WebP, BMP support with quality control and resize options
- **Video compression** — Smart mode (target size in MB) or Manual mode (CRF + resolution)
- **No FFmpeg install needed** — uses `imageio-ffmpeg` bundled binary
- **Live progress bar** during video encoding
- **Before/After size metrics** after every compression
- **One-click download** of compressed file
- Runs 100% locally — no data leaves your machine

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/mediacrush.git
cd mediacrush
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the app

```bash
streamlit run main.py
```

The app will open automatically at `http://localhost:8501`

---

## 📦 Requirements

| Package | Purpose |
|---|---|
| `streamlit` | Web app framework |
| `Pillow` | Image processing |
| `imageio-ffmpeg` | Bundled FFmpeg binary for video compression |

---

## 🖼️ Image Compression

- Supported formats: JPG, JPEG, PNG, WebP, BMP
- Adjust **JPEG quality** (10–95)
- Set **max width** to resize large images
- Choose **output format**: JPEG, PNG, or WEBP

## 🎬 Video Compression

**Smart Mode** — set a target size in MB and the app auto-picks the best resolution and CRF value.

**Manual Mode** — full control:
- CRF (18 = best quality, 28 = balanced, 35 = smallest file)
- Resolution: 1920×1080, 1280×720, 854×480, 640×360
- Encoding speed preset: ultrafast → veryslow

---

## 📁 Project Structure

```
mediacrush/
├── main.py            # Streamlit app
├── requirements.txt   # Python dependencies
├── README.md          # This file
└── .gitignore         # Files to exclude from git
```

---

## 🙈 .gitignore

See `.gitignore` — temporary files and Python cache are excluded automatically.

---

## 📄 License

MIT License — free to use, modify, and distribute.
