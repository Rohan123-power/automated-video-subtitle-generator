# Automated Video Subtitle Generator

AI-powered video subtitle generator using Python, Streamlit, Whisper, and FFmpeg.

---

# Features

- Upload video files
- Extract audio from videos
- Automatically generate subtitles
- Generate `.srt` and `.vtt` subtitle files
- Embed subtitles into videos
- Simple Streamlit-based user interface

---

# Technologies Used

- Python
- Streamlit
- OpenAI Whisper
- FFmpeg
- NumPy
- MoviePy

---

# Project Workflow

1. Upload video file
2. Extract audio using FFmpeg
3. Convert speech to text using Whisper
4. Generate subtitle files
5. Merge subtitles with video
6. Download subtitled video

---

# Project Structure

```text
Auto-Subtitled-Video-Generator-master/
│
├── pages/
│   ├── 02_📼_Upload_Video_File.py
│   └── local/
│
├── utils.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── venv/   (ignored)
```

---

# Installation

## 1. Clone Repository

```bash
git clone <your-github-repository-link>
cd Auto-Subtitled-Video-Generator-master
```

---

## 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate virtual environment:

### Windows

```bash
venv\Scripts\activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# FFmpeg Installation

This project requires FFmpeg.

Download FFmpeg from:

https://www.gyan.dev/ffmpeg/builds/

After installation:

1. Extract FFmpeg
2. Copy the FFmpeg `bin` folder path
3. Add it to Windows Environment Variables PATH

Verify installation:

```bash
ffmpeg --version
```

---

# Run Application

Run the Streamlit application using:

```bash
streamlit run "pages/02_📼_Upload_Video_File.py"
```

---

# Supported Formats

- MP4
- AVI
- MOV
- MKV

---

# Output Files

The application generates:

- transcript.txt
- transcript.srt
- transcript.vtt
- subtitled video (.mp4)

---

# Notes

- Whisper base model is recommended for faster processing.
- Large Whisper models provide higher accuracy but slower performance.
- FFmpeg must be installed separately.

---

# Author

Developed using Python, Streamlit, Whisper AI, and FFmpeg.
