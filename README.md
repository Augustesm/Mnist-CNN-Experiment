# MNIST CNN Experiment

This project explores the creation, training, and evaluation of **Convolutional Neural Networks (CNNs)** using the MNIST handwritten digits dataset. The work focuses on experimenting with different CNN architectures by adjusting hyperparameters such as convolution filter sizes, number of filters, pooling layers, optimizers, dense layers, and learning rates. The goal is to compare multiple CNN variants (5 or more) and evaluate their performance against the best previously built fully connected neural network.

---

## 📌 Key Features

* 🧠 Implementation of multiple custom CNN architectures
* 🔍 Hyperparameter experiments (filters, pooling, learning rate, epochs, optimizers)
* 📊 Tracking training accuracy, validation accuracy, test accuracy, and losses
* 📝 Results summary table for all tested model variants
* 🔢 Automatic recognition of user-drawn digits (e.g., *Sample7.png*)
* 🖼️ Visualization of misclassified images
* ⚖️ Comparison with fully connected neural network accuracy

---

## 🛠️ Technologies Used

* **Python**
* **TensorFlow / Keras**
* **NumPy**
* **Matplotlib**
* **Pillow (PIL)** for loading custom images

---

## 🔧 Model Architecture (Base Version)

* `Input(shape=(28, 28, 1))`
* `Conv2D` layers with different filter counts and kernel sizes
* `AveragePooling2D` and `MaxPooling2D` layers depending on experiment
* `Flatten` for feature vector transformation
* Fully connected `Dense` layers
* Output layer with `softmax` activation for 10-class classification

---

## 📈 Training Setup

* **Optimizer:** Adam (learning rate adjustable)
* **Loss:** Categorical Crossentropy
* **Batch Size:** 32
* **Epochs:** 6+
* **Validation Split:** 20%

The project includes graphs showing model accuracy and loss during training and validation.

---

## 🧪 Evaluation & Testing

* Automatic prediction for test images
* Extraction of misclassified digits
* Visualization of incorrect predictions
* Prediction for custom user-uploaded images such as `"Sample7.png"`
* Table summarizing each model variant with:

  * Hyperparameters changed
  * Training accuracy
  * Validation accuracy
  * Test accuracy
  * Loss values
  * Whether the handwritten digit was recognized correctly
