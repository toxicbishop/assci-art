# assci-art

Play video as ASCII art in your terminal.

<!-- Demo video: replace assets/demo.mp4 with your demo file or a hosted URL -->
<video src="assets/vid.mp4" controls width="640">Your browser does not support the video tag.</video>


## Prerequisites
- Python 3.8 or newer
- Git (optional)

## Required: use a virtual environment
This project must be used inside an isolated venv.

Windows (PowerShell)
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Windows (cmd)
```cmd
python -m venv .venv
.venv\Scripts\activate.bat
```

macOS / Linux
```bash
python3 -m venv .venv
source .venv/bin/activate
```

## Install dependencies
With the venv activated:
```bash
pip install --upgrade pip
pip install numpy opencv-python
```
(Optional) save requirements:
```bash
pip freeze > requirements.txt
```

## Run
```bash
python index.py
```
Follow prompts for the video path, terminal width and FPS.

Or run non-interactively:
```bash
python -c "from index import play_video_in_terminal; play_video_in_terminal('path/to/video.mp4', width=80, fps=30)"
```