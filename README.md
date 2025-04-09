# **Digit Classification with Convolutional Neural Networks (CNN)**

## **Project Overview**
In this project, we aim to classify handwritten digits (from 0 to 9) using Convolutional Neural Networks (CNNs). The dataset used for this task is the **Digits dataset** from Scikit-learn, which contains 1797 8x8 pixel grayscale images of handwritten digits, with each image labeled according to the digit it represents. Our goal is to preprocess the data, build a CNN model for digit classification, evaluate its performance, and visualize the results.

## **Steps Taken in the Project**
1. **Data Loading & Preprocessing**: The dataset is loaded using the `load_digits()` function from Scikit-learn. Each image is resized to 32x32 pixels, and pixel values are normalized to lie between 0 and 1 for better model performance.

2. **Model Building**: We build a Convolutional Neural Network (CNN) using **TensorFlow** and **Keras**, consisting of two convolutional layers followed by max-pooling layers, a flattening layer, and fully connected layers. The model is designed to classify the 10 possible digits (0-9).

3. **Model Training**: The CNN is trained on the preprocessed dataset for 15 epochs, with a validation split of 10%. The training process is visualized with graphs showing accuracy and loss over the epochs for both training and validation sets.

4. **Model Evaluation**: After training, we evaluate the model's performance on the test set using various metrics, including **accuracy**, **precision**, **recall**, **F1-score**, and a **confusion matrix**. We also visualize the **per-class accuracy** to see how well the model performs on each digit.

5. **Error Analysis**: We analyze the errors by visualizing the misclassified images, along with their true and predicted labels. This helps us identify any patterns or digits that the model struggles with.

6. **Prediction Probabilities**: For an example image, we visualize the model's predicted probabilities for each digit, providing insight into the model's confidence for each class.
