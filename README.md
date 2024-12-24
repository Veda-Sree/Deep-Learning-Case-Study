The code implements a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset. Here's a breakdown of its functionality:

1. Data Preprocessing:  
   - Loads the MNIST dataset of handwritten digits.  
   - Normalizes pixel values to range between 0 and 1.  
   - Expands dimensions for compatibility with CNN input.  
   - Converts labels to one-hot encoded format.

2. CNN Model:  
   - Sequential CNN architecture with:  
     - Three convolutional layers (Conv2D) with ReLU activation.  
     - MaxPooling layers to downsample feature maps.  
     - A Flatten layer to prepare data for the dense layer.  
     - Two dense layers: one hidden layer with 128 neurons and an output layer with 10 neurons (softmax activation for digit classification).  

3. Model Training and Evaluation:  
   - Compiles the model using the Adam optimizer and categorical crossentropy loss.  
   - Trains the model for 5 epochs with a batch size of 64, using 20% of the training data for validation.  
   - Evaluates the model on the test set, calculating metrics like accuracy and generating a confusion matrix, classification report, precision, recall, and F1 scores.

4. Results Reporting:  
   - Prints overall and class-wise metrics, including confusion matrix, classification report, precision, recall, and F1 scores for all 10 classes (digits 0–9).  

