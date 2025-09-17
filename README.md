\# Human Figure Drawing IQ Estimator



This project implements an AI-based system to classify children's cognitive levels from their Human Figure Drawings (HFDs) based on the DAP (Draw-A-Person) approach.

It predicts one of four IQ levels: \*\*Very Low (0), Low (1), Average (2), High (3)\*\*.



---



\##  Overview

\- \*\*Input:\*\* A child's human figure drawing (image)

\- \*\*Output:\*\* One of four cognitive levels: `Very Low`, `Low`, `Average`, or `High`

\- \*\*Models Used:\*\* MobileNet, MobileNetV2, InceptionV3, Xception

\- \*\*Best Model Result:\*\* InceptionV3 — \*\*80.22% accuracy\*\*

## Dataset

The dataset used for this project consists of **approximately 1,900 human figure drawings**:

- **~1,000 images** collected manually from schools in Syria over the years 2024–2025.  
  These images were carefully processed and **manually labeled** according to cognitive levels.
- **~900 images** sourced from an online repository.  

> Note: For privacy reasons, the full dataset is not included in this repository.  
> An **example dataset** is provided in `data/example/` to illustrate the required format (`image_path`, `label`).

All images are labeled with cognitive levels:  
**0 = Very Low, 1 = Low, 2 = Average, 3 = High**.




---



\##  Project Structure

HumanFigureDrawing-IQ-Estimator/

│

├── README.md
├── LICENSE
├── requirements.txt
├── data/
│   └── examples
├── src/
│ ├── IQ_project.py





---



\## Installation

Make sure you have Python 3.8+ installed.



```bash

git clone https://github.com/YOUR\\\_USERNAME/HumanFigureDrawing-IQ-Estimator.git

cd HumanFigureDrawing-IQ-Estimator

pip install -r requirements.txt



Main dependencies:

TensorFlow / Keras

scikit-learn

pandas

numpy

matplotlib

os

ImageDataGenerator (from Keras)



Train the model on your dataset:
python src/train.py



Evaluate the trained model:
python src/evaluate.py



The dataset should be defined in labels.csv linking each image to its IQ class (0–3).





