### Image Classification Using Keras

This project demonstrates how to build and train a convolutional neural network (CNN) to classify images using the Keras library. It was completed as part of the Fundamentals of Python Programming (PPY) course during my Computer Science studies at the Polish-Japanese Academy of Information Technology (PJAIT).

The process involves several key steps, which are outlined below:

#### 1. Data Preparation
- **Loading the Dataset**: The training data, containing image paths and their corresponding labels, is loaded from a CSV file.
- **Processing Images**: Each image is loaded and resized to a consistent size (e.g., 28x28 pixels) with 3 color channels (RGB). The images are then converted into numpy arrays and normalized to a range of 0-1.
- **Preparing Labels**: The image labels are converted into a one-hot encoded format to facilitate training.

#### 2. Splitting the Data
- The dataset is split into training and validation sets to enable model training and performance evaluation.

#### 3. Building the Model
- A sequential CNN model is defined, consisting of:
  - Convolutional layers with ReLU activation to detect features in the images.
  - A max-pooling layer to reduce the spatial dimensions of the feature maps.
  - A flatten layer to convert the 2D feature maps into a 1D vector.
  - Dense (fully connected) layers, with the final layer using softmax activation to classify the images into multiple categories.

#### 4. Training the Model
- The model is trained on the training dataset and validated using the validation set. Training typically occurs over multiple epochs to optimize the model's weights and improve accuracy.

#### 5. Model Evaluation and Prediction
- **Loading the Test Data**: Similar to the training data, the test dataset is loaded and processed.
- **Evaluating the Model**: The model's performance is evaluated using the test set to determine its accuracy and loss.
- **Making Predictions**: The trained model is used to predict the classes of images in the test set.

#### 6. Displaying Results
- The results for selected images from the test set are displayed, showing the actual and predicted labels to illustrate the model's performance.
