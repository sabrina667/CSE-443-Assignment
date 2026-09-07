# Pneumonia Detection Using CNN

## Objective

The objective of this problem is to develop a Convolutional Neural Network (CNN) model to classify chest X-ray images into two classes:

- Normal
- Pneumonia

## Dataset

The dataset contains chest X-ray images of pediatric patients. The images are divided into training, validation, and testing sets.

The target classes are:

- Normal
- Pneumonia

## Methodology

The following steps were performed:

1. Loaded the chest X-ray dataset.
2. Checked the dataset structure and class distribution.
3. Visualized sample chest X-ray images.
4. Resized the images to 150 × 150 pixels.
5. Normalized pixel values to the range 0 to 1.
6. Applied data augmentation to the training images.
7. Created a Convolutional Neural Network.
8. Used convolutional and max-pooling layers to extract image features.
9. Used a fully connected layer and dropout.
10. Used a sigmoid output layer for binary classification.
11. Trained the model using the training dataset.
12. Evaluated the model using the validation and test datasets.
13. Generated a confusion matrix and classification report.
14. Calculated accuracy, precision, recall, and F1-score.
15. Saved the trained CNN model.

## CNN Architecture

The CNN consists of:

- Convolutional layers
- Max Pooling layers
- Flatten layer
- Dense layer
- Dropout layer
- Sigmoid output layer

The model uses the Adam optimizer and binary cross-entropy loss function.

## Data Preprocessing

The images were resized to **150 × 150 pixels**.

Pixel values were normalized to the range **0 to 1**.

Data augmentation was applied to the training images using:

- Rotation
- Zoom
- Shearing
- Horizontal flipping

## Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Results

The model achieved the following results on the test dataset:

| Metric | Result |
|---|---:|
| Test Loss | 0.4061 |
| Test Accuracy | 80.13% |
| Precision | 77.25% |
| Recall | 96.67% |
| F1 Score | 85.88% |

### Confusion Matrix

```text
[[123 111]
 [ 13 377]]
The model correctly classified 123 Normal images and 377 Pneumonia images.

It incorrectly classified 111 Normal images as Pneumonia and 13 Pneumonia images as Normal.

Technologies Used
Python
TensorFlow
Keras
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
Google Colab
Conclusion

A CNN model was successfully developed for classifying chest X-ray images into Normal and Pneumonia categories.

The model achieved 80.13% test accuracy, 77.25% precision, 96.67% recall, and 85.88% F1-score.

The experiment demonstrates that CNNs can learn useful visual patterns from medical images and perform image classification.

This project is intended for academic purposes and should not be considered a clinical diagnostic system.
