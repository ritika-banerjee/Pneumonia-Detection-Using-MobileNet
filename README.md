# Pneumonia Detection using Chest X-ray Images

This project uses a Convolutional Neural Network (CNN) to classify chest X-ray images as either pneumonia-positive or normal. The model is trained and evaluated on the [Chest X-ray Images (Pneumonia) dataset by Paul Timothy Mooney](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), available on Kaggle.

## Dataset
The dataset contains X-ray images divided into `train`, `validation`, and `test` sets. Images are preprocessed and augmented to improve model generalization.

### Directory Structure
- `train/`: Contains training images.
- `val/`: Contains validation images.
- `test/`: Contains test images.

Ensure these directories match the paths specified in the script.

## Installation

1. Clone this repository and navigate to the project directory.
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
3.Download the dataset from Kaggle using
  ```bash
  kaggle datasets download -d paultimothymooney/chest-xray-pneumonia
```

## Project Structure

- Data Augmentation: The project uses ImageDataGenerator from Keras to apply transformations such as rotations, zooms, and flips to increase dataset diversity.
- Model Architecture: A CNN model with binary classification capabilities is built and compiled using Keras. Training is monitored using TensorBoard.
- Callbacks: Early stopping and learning rate adjustments are implemented to optimize training performance.

## Results
Saved model weights are stored in `best_model.keras.`
Training and validation metrics are plotted for loss and accuracy.

## Acknowledgments
Dataset: Kaggle - Chest X-ray Images (Pneumonia)
