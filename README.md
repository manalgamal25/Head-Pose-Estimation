# Head Pose Estimation

A machine learning project that estimates head pose (pitch, yaw, roll) from facial landmarks using MediaPipe Face Mesh and Support Vector Regression (SVR).

## Overview

This project uses:
- **MediaPipe Face Mesh**: To extract 468 facial landmark points
- **Support Vector Regression (SVR)**: To predict head pose angles (pitch, yaw, roll) from facial landmarks

## Features

- Extract facial landmarks from images using MediaPipe
- Train SVR models for pitch, yaw, and roll estimation
- Visualize head pose with 3D axis overlay
- Process images and videos

## Installation

1. Clone this repository:
```bash
git clone <repository-url>
cd Head_Pose_estimation
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## Dataset

Download the AFLW2000-3D dataset from:
http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/Database/AFLW2000-3D.zip

Extract it to the project directory. The dataset should be in the `AFLW2000` folder.

## Usage

1. Open the Jupyter notebook: `Head_Pose_estimation_.ipynb`

2. Run the cells in order:
   - Import libraries
   - Load and process the dataset
   - Train the models
   - Test on images or videos

3. For video processing, update the `INPUT_VIDEO` variable in the notebook with your video path.

## Project Structure

```
Head_Pose_estimation/
├── Head_Pose_estimation_.ipynb  # Main notebook
├── requirements.txt              # Python dependencies
├── README.md                     # This file
├── .gitignore                    # Git ignore rules
└── AFLW2000/                     # Dataset directory (not included in repo)
```

## Requirements

- Python 3.7+
- numpy
- opencv-python
- scipy
- scikit-learn
- mediapipe

## Notes

- The dataset files are not included in the repository (see `.gitignore`)
- Make sure to download and extract the AFLW2000-3D dataset before running the notebook
- For video processing, ensure you have sufficient memory as all frames are loaded into memory

## License

[Add your license here]

## Author

[Add your name/contact here]

