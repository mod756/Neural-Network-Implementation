# Neural Network Implementation using TensorFlow and Keras
# Features
+ A simple feedforward neural network implemented using TensorFlow and Keras.
+ Incorporates EarlyStopping and ModelCheckpoint callbacks to prevent overfitting and save the best model during training.
+ Achieves high accuracy on the MNIST dataset (handwritten digit recognition).
+ Training and validation accuracy/loss are visualized in real-time using Matplotlib.
# Dataset
**MNIST dataset:** Consists of 60,000 training images and 10,000 test images, where each image is a 28x28 grayscale picture of handwritten digits (0-9).

TensorFlow automatically normalizes the pixel values to the range [0, 1] to improve performance.

# Workflow
**Data Loading:** 
+ The MNIST dataset is loaded using TensorFlow’s datasets API.

**Data Preprocessing:**
+  Images are normalized, and labels are one-hot encoded for multi-class classification.

**Model Definition:** 

A feedforward neural network is built using Keras’s Sequential API:
+ Input layer (flattened 28x28)
+ Two hidden layers with ReLU activations
+ Output layer with softmax activation for classification.

**Training:**

+ Model is compiled using the Adam optimizer and categorical cross-entropy loss.
+ EarlyStopping and ModelCheckpoint callbacks are used to optimize training.
+ Training progress is visualized with real-time plots showing accuracy and loss for both training and validation data.

**Evaluation:**
+  The best model (saved in .keras format) is evaluated on the test set, achieving a high accuracy (~98%).

# Conclusions Drawn
+ The neural network performs effectively on the MNIST dataset, achieving high accuracy.
+ Real-time training visualization helps monitor the model’s performance and diagnose potential overfitting.
+ EarlyStopping and ModelCheckpoint were key in saving the best-performing model and avoiding overfitting.
