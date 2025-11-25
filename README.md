# MNIST Handwritten Digit Classification

---

## Project Overview
Built an **Artificial Neural Network (ANN)** to classify handwritten digits from the MNIST dataset. The workflow includes **data preprocessing, model building, training, evaluation, and model persistence**.

---

## Dataset
- **Source:** `tensorflow.keras.datasets.mnist`
- **Train/Test Split:** 60,000 / 10,000 images
- **Image Shape:** 28x28 grayscale
- **Classes:** 10 digits (0–9)

---

## Workflow
1. **Data Preprocessing:**  
   - Normalized pixel values to [0,1].  
   - One-hot encoded labels.
2. **Model Architecture:**  
   - Input: Flatten layer.  
   - Hidden layers: Dense (128 → 64 neurons) with ReLU and Dropout (0.3).  
   - Output: Dense layer with Softmax for 10 classes.
3. **Compilation:** Optimizer: Adam, Loss: Categorical Crossentropy, Metrics: Accuracy.
4. **Training:** 10 epochs, batch size 128, 10% validation split.
5. **Evaluation:** Accuracy, confusion matrix, classification report on test set.
6. **Visualization:** Training/validation accuracy plots and confusion matrix heatmap.
7. **Model Persistence:** Saved and reloaded model in HDF5 format.

---

## Skills Demonstrated / Concepts Applied
- **Deep Learning & ANN Design:** Built ANN using Keras Sequential API with dense layers.
- **Data Preprocessing:** Normalized pixel values and converted labels to one-hot encoding.
- **Feature Engineering:** Flattened 28x28 images to 1D arrays for ANN input.
- **Activation Functions & Regularization:** Used ReLU for hidden layers, softmax for output layer, and applied Dropout to prevent overfitting.
- **Training & Backpropagation:** Trained the network using Adam optimizer and categorical crossentropy loss (backpropagation handled by Keras).
- **Hyperparameter Tuning:** Selected number of epochs, batch size, and dropout rates to optimize performance.
- **Model Evaluation:** Measured performance using accuracy, confusion matrix, and classification report; visualized training/validation accuracy.
- **Model Persistence:** Saved and reloaded trained model (.h5) for reproducibility.

---

## Outputs / Visualizations
- Sample digit images with labels
- Training and validation accuracy plots
- Confusion matrix heatmap
- Classification report metrics
---
