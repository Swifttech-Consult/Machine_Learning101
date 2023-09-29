# Machine_Learning101

ML Assessment Solution

Author: Anthony Akore
Email: anthony.akore@workwithaya.com

This code is a solution for a machine learning assessment. It performs the following tasks:

Step 1: Data Preparation and Exploration
------------------------------------------

1. Mounts Google Drive to access the dataset.
2. Loads the dataset from Google Drive located at "/content/gdrive/MyDrive/Covid."
3. Creates a dataset from the directory for both training and validation.
   - Images are resized to (224, 224) pixels.
   - Batch size is set to 64.
   - Validation split is 80% for training and 20% for validation.
4. Displays a sample of the dataset with labels.

Step 2: CNN Model Definition, Training, and Evaluation
------------------------------------------------------

1. Defines a Convolutional Neural Network (CNN) model for binary classification (COVID-19 or not). The model consists of:
   - Convolutional layers with ReLU activation.
   - MaxPooling layers.
   - Dense layers with ReLU activation.
   - A dropout layer to prevent overfitting.
   - The output layer with a sigmoid activation function.
2. Applies data augmentation to the model using random horizontal flipping, rotation, and zoom.
3. Compiles the model using the Adam optimizer and binary cross-entropy loss.
4. Trains the model for 10 epochs using the training dataset while collecting accuracy values.
5. Evaluates the model on the validation dataset, collecting true and predicted labels.

Step 3: Metrics Calculation and Visualization
---------------------------------------------

1. Calculates accuracy, precision, recall, and F1-score for the model's predictions.
2. Stores and visualizes training and validation accuracy values over epochs.
3. Displays accuracy, precision, recall, and F1-score values.
4. Prints true labels and predicted labels for each image.

To run this code, make sure to have the required libraries installed and adjust the dataset directory path accordingly. You can also modify the model architecture and training parameters as needed.

