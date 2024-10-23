
# OncoVision

OncoVision is a deep learning Convolutional Neural Network (CNN) model designed to detect brain tumors using MRI images. This model classifies MRI images into two categories: "Tumor Positive" or "Healthy". By leveraging deep learning, OncoVision aims to provide an efficient and accurate method for tumor detection, potentially aiding in the early diagnosis and treatment of brain tumors.


## Dataset API

```python
import kagglehub

# Download latest version
path = kagglehub.dataset_download("navoneel/brain-mri-images-for-brain-tumor-detection")
print("Path to dataset files:", path)
```
## Features

* **Deep Learning Model:** Uses a CNN architecture to classify MRI images.
* **Image Preprocessing:** Images are resized and processed to ensure compatibility with the model.
* **High Accuracy:** Achieves competitive accuracy and F1 scores for tumor detection.
*  **Prediction Output:** Provides the prediction labels for the uploaded  MRI images: either "Tumor Positive" or "Healthy".
## Installation

To use OncoVision, follow these steps:

1. **Clone the Repository**
```bash
    git clone https://github.com/priyanathbhukta/oncovision.git
    cd oncovision
```
2. **Install dependencies**
```bash
    pip install -r requirements.txt
```
3. **Run the Model:** Once dependencies are installed, you can start using the model to classify MRI images.
    
## Usage

To use the model for MRI image classification, follow these steps:
1. **Load MRI images:** Organize your MRI images into two folders:
    * `yes/` for tumor-positive images
    * `no/` for healthy images
2. **Run the Script:** The script will preprocess the images, run predictions using the CNN model, and output the results for each image.
3. **View Results:** The model will print out the prediction for each image, whether it is "Tumor Positive" or "Healthy". It will also display overall metrics like accuracy.




## Model Evaluation
The performance of OncoVision is evaluated using two key metrics:

*   **Accuracy:** The proportion of correct predictions (both "Tumor Positive" and "Healthy") to the total number of predictions.
```bash
    accuracy = (correct_predictions / total_images) * 100

```
* **F1-Score:** The harmonic mean of precision and recall, which gives a balanced measure of the model's performance, especially useful in imbalanced datasets.
```bash
    f1_score = 2 * (precision * recall) / (precision + recall)
```
## Contributing

We welcome contributions to improve OncoVision. Please fork the repository and submit pull requests for any enhancements or bug fixes.

