## Dog Breed Classification Using CNN

This project implements a Convolutional Neural Network (CNN) to classify dog breeds from images. The dataset, developed by me, can be found on Kaggle: [Dog Breed Classification Dataset](https://www.kaggle.com/datasets/khushikhushikhushi/dog-breed-image-dataset)).

### Steps:

1. **Loading and Preprocessing**:
    - Images are loaded and resized to 150x150 pixels.
    - Labels are encoded and converted to one-hot vectors.
    - The dataset is split into training and validation sets (80-20 split).

2. **Defining the CNN Model**:
    - Three convolutional layers, each followed by a max-pooling layer.
    - A fully connected dense layer with dropout regularization.
    - Softmax activation for multi-class classification.

3. **Training the Model**:
    - Compiled with categorical cross-entropy loss and the Adam optimizer.
    - Trained for 30 epochs with a batch size of 32.
    - Training and validation accuracy are monitored.

4. **Evaluating and Saving the Model**:
    - Evaluated on the validation set.
    - Saved as `dog_breed_classifier_model.h5`.

5. **Making Predictions**:
    - Function to predict the breed of a random image from the validation set.
    - Displays the image, its actual breed, and the predicted breed.

