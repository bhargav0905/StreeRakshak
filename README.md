# Emotion Detection Using CNN

This project implements an emotion detection system using Convolutional Neural Networks (CNN). The system is trained on the FER2013 dataset and can identify various facial expressions.

## Installation

Before proceeding, ensure you have Python installed on your system. Use the following commands to install the required packages:

```bash
pip install numpy
pip install opencv-python
pip install keras
pip3 install --upgrade tensorflow
pip install pillow
```

## Dataset

Download the FER2013 dataset from the link below:

[FER2013 Dataset](https://www.kaggle.com/msambare/fer2013)

Place the downloaded dataset into a `data` folder within your project directory.

## Training the Emotion Detector

Train the emotion detection model using the FER2013 dataset. Use the following command:

```bash
python TrainEmotionDetector.py
```

### Notes:
- Training time may vary depending on your system specifications. For reference, it took approximately 4 hours on an Intel i7 processor with 16 GB RAM.
- After training, the model's structure and weights will be saved in your project directory as:
  - `emotion_model.json`
  - `emotion_model.h5`

### Post-Training Setup:
1. Create a folder named `model` in your project directory.
2. Move the `emotion_model.json` and `emotion_model.h5` files to the `model` folder.

## Testing the Emotion Detector

To test the trained emotion detection model, execute the following command:

```bash
python TestEmotionDetector.py
```

## Project Directory Structure

Ensure your project directory is structured as follows:

```
Emotion_detection_with_CNN/
|
├── data/
│   └── fer2013.csv  # FER2013 dataset
|
├── model/
│   ├── emotion_model.json
│   └── emotion_model.h5
|
├── TrainEmotionDetector.py
├── TestEmotionDetector.py
└── README.md
```

## Additional Information

- Verify that your Python environment has adequate resources allocated for training.
- For any questions or issues, feel free to open an issue in the repository.
