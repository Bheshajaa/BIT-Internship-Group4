# BIT-Internship-Group4
Deep learning internship Face Recognition project

##**Importing Required Libraries**:

The code imports necessary libraries like pandas, os, glob, and TensorFlow's Keras module.

##**Assigning Path for Dataset:**
Defines paths for training and testing datasets.

##**Checking Number of Categories and Images:**
Iterates through the training and testing directories, counting the number of images in each category.

##**Displaying Random Images:**
Defines a function view_random_image to display a random image from a specified directory with its corresponding class label.
Uses Matplotlib to display a grid of random images from different classes.

##**Preparing Data for Training:**
Uses Keras' ImageDataGenerator to augment and preprocess training and testing data.
Flow_from_directory is used to create generators for the training and testing sets.

##**Basic Model Building (CNN Classifier):**
Initializes a Sequential model.
Adds convolutional layers with max-pooling to extract features.
Flattens the output and adds fully connected layers.
Compiles the model using the Adam optimizer and categorical cross-entropy loss.

##**Training the Model:**
Trains the model using the training set and validates on the test set for 50 epochs.

##**Saving the Model:**
Saves the trained model to a file named 'model1.h5'.

##**Evaluating the Model:**
Evaluates the model on the test set and prints the loss and accuracy.

##**Plotting Training History:**
Plots the training and validation loss and accuracy over epochs.

##**Loading the Model:**
Loads the saved model from the 'model1.h5' file.

##**Making Predictions:**
Reads an image using OpenCV, resizes it to the required dimensions, and preprocesses it.
Uses the loaded model to make predictions on the preprocessed image.

##**Displaying Predictions:**
Prints the predicted class index and maps it to the corresponding emotion using the class indices from the training set.
The code essentially performs the following tasks: data preparation, model building, training, evaluation, and making predictions on a sample image. The model is a basic Convolutional Neural Network (CNN) for emotion detection based on images.

OUTPUT:
![Screenshot 2023-11-24 000946](https://github.com/Bheshajaa/BIT-Internship-Group4/assets/142480959/0255a2f3-f280-43ca-9a3e-22002aaf9b33)
![Screenshot 2023-11-24 001143](https://github.com/Bheshajaa/BIT-Internship-Group4/assets/142480959/067311d8-15f2-4788-a88e-ea2017522608)
![Screenshot 2023-11-24 002047](https://github.com/Bheshajaa/BIT-Internship-Group4/assets/142480959/42f9057c-eaa3-495d-a76c-698a8c29d3d2)
