# Coverdrive_analyser-

# 🏏 Cover Drive Analyzer using OpenCV & MediaPipe

Welcome to the **Cover Drive Analyzer**, a computer vision project that evaluates a cricket player’s cover drive shot using pose estimation and custom scoring logic. Built using Python, OpenCV, and MediaPipe, this project aims to assist players, coaches, and enthusiasts in analyzing and improving shot techniques by focusing on key biomechanical aspects.

## 📌 Features

- 🎯 Pose estimation using **MediaPipe Holistic**
- 🧍‍♂️ Keypoint extraction for body pose analysis
- 📝 Scoring mechanism based on:
  - Footwork
  - Balance
  - Bat swing
  - Head position
  - Follow-through
- 🧠 Feedback generation with visual overlays on key frames
- 📊 JSON/text output summarizing performance

## 🎥 Sample Output

<img src="sample_frame.png" width="600"/>

{
"Footwork": 8,
"Balance": 9,
"Bat Swing": 7,
"Head Position": 9,
"Follow-through": 8,
"Comments": "Good control and head stability. Improve bat swing smoothness for better timing."
}

markdown
Copy
Edit

## 🛠️ Technologies Used

- Python
- OpenCV
- MediaPipe
- NumPy
- Matplotlib (for plotting key frames)

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cover-drive-analyzer.git
   cd cover-drive-analyzer
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the analyzer

bash
Copy
Edit
python cover_drive_analyzer.py --input coverdrive.mp4
Output

Pose-annotated video

Frame-wise feedback

Final JSON/text summary

📂 Folder Structure
bash
Copy
Edit
📁 cover-drive-analyzer
│
├── 📁 data/              # Input videos/images
├── 📁 outputs/           # Results with annotated frames and JSON
├── 📜 cover_drive_analyzer.py
├── 📜 scoring_logic.py
├── 📜 utils.py
├── 📄 requirements.txt
└── 📄 README.md
🧠 Scoring Logic
The analyzer evaluates each shot based on key biomechanical parameters. The final scores are normalized on a 10-point scale with heuristic thresholds based on joint positions and motion fluidity.

🙌 Future Scope
Train a model using labeled shot data for more accurate scoring.

Add comparison with professional players.

Export insights to coaching dashboards.

🧑‍💻 Author
Parth Dhamdhere
📫 LinkedIn
📧 parth@example.com
