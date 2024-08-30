# EmoSense: Advanced Emotion Recognition System for Group Photos

## Overview

EmoSense is an advanced emotion recognition system designed to identify individual emotions within group photos. The solution leverages state-of-the-art deep learning techniques, including YOLO (You Only Look Once) for real-time face detection and DeepFace for emotion classification, to provide a nuanced understanding of group dynamics by analyzing each individual's emotional state.

## Key Features

- **Robust Face Detection**: Uses YOLOv8 face detection model to accurately detect multiple faces within diverse group settings, such as company events, school assemblies, or community gatherings.
- **Emotion Recognition**: Utilizes DeepFace library to classify emotions like happy, sad, neutral, angry, etc., for each detected face.
- **Scalable Solution**: Designed to handle large datasets efficiently with batch processing and modular components.
- **Improvement Analysis**: Evaluates the impact of super-resolution techniques on emotion recognition confidence scores.

## Project Structure

- **`EmoSense_Project_CVII.ipynb`**: Jupyter Notebook containing the full implementation of the solution, including face detection, emotion recognition, and evaluation.
- **`emosense_project_cvii.py`**: Python script version of the implementation for running the solution outside Jupyter Notebook.
- **`Project_Emosense.pdf`**: Detailed project report covering the implementation process, challenges, solutions, results, and future improvements.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/EmoSense.git
   cd EmoSense
Usage
1. Running the Jupyter Notebook
  Open EmoSense_Project_CVII.ipynb in Jupyter Notebook or Google Colab.
2. Follow the instructions in the notebook to:
  Perform face detection on group images using YOLO.
  Extract and classify individual emotions using DeepFace.
  Analyze results and visualize confidence score distributions.

2. Install the required dependencies:
  pip install -r requirements.txt
3. Running the Python Script(python emosense_project_cvii.py)
The script will:
  Detect faces in the input images. but make sure to change your own directory intact where u want to save)
  Extract and classify emotions for each face.
  Save results to CSV files for further analysis.

Evaluation
  Results: Preliminary results indicate high accuracy in detecting individual emotions within groups, with confidence scores predominantly above 80%.
  Metrics: The project uses confidence scores as a metric for evaluation, given the lack of labeled data.
  Visualization: Includes histograms and box plots to compare confidence scores before and after applying super-resolution techniques.
  
Challenges and Solutions

  Lack of Labeled Data: Confidence scores were used as a proxy metric due to the unavailability of labeled data.
  Handling Overlapping Faces: YOLO was chosen for its ability to detect multiple, overlapping faces at different scales.
  Efficient Processing: Implemented batch processing to handle large datasets effectively.

Future Enhancements
  Incorporate advanced super-resolution models to improve emotion recognition accuracy.
  Explore ensemble methods combining multiple emotion recognition models.
  Add real-time video processing capabilities for live event analysis.

How to Contribute:
---------------------
  
We welcome contributions to enhance EmoSense! Here’s how you can contribute:

  1. Fork the repository.
  
  2. Create a new branch (git checkout -b feature-branch).
  
  3. Make your changes.
  
  4. Commit your changes (git commit -am 'Add new feature').
  
  5. Push to the branch (git push origin feature-branch).
  
  6. Open a pull request.
