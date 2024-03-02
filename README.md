# TensorFlow-Basics-Implementation-in-Python_Cat-Image-Classification

The provided code involves building a convolutional neural network (CNN) to classify images as either "cat" or "non-cat". Here's a breakdown of what each part of the code does:

1. **TensorFlow and Keras Imports**: The code begins with importing necessary modules from TensorFlow and Keras, including layers for building neural networks and utilities for image preprocessing.

2. **Model Definition**: It defines a CNN model using Keras's Sequential API. The model consists of convolutional layers (`Conv2D`), max-pooling layers (`MaxPooling2D`), and fully connected layers (`Dense`). The final layer uses a sigmoid activation function, suitable for binary classification problems.

3. **Model Compilation**: The model is compiled with an Adam optimizer and binary cross-entropy loss function. It also specifies accuracy as a metric to monitor during training.

4. **Data Preparation**: Dummy data is created since there's no dataset available. The same image (repeated 100 times) is used for both features and labels. Then, the data is split into training and validation sets.

5. **Data Augmentation**: Image data generators (`ImageDataGenerator`) are created for both training and validation data. Data augmentation techniques like rotation, shifting, shearing, zooming, and horizontal flipping are applied to the training data. Validation data is not augmented.

6. **Model Training**: The model is trained using the `fit` method. Training and validation data generators are provided to train the model.

7. **Prediction and Visualization**: After training, the model makes predictions on a sample image (`Cats.jpg`) and visualizes the result along with the image. It also saves the model for future use.

8. **Model Evaluation**: The saved model is loaded, and then, predictions are made on a random image (`dog.jpg`). The prediction label, confidence, and prediction value are printed, and the image with the prediction label is visualized.
