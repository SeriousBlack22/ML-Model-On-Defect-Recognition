# ML-Model-On-Defect-Recognition

Trainer Code:

The trainer code is responsible for preparing and training the crack detection model.

Data Preparation:

Loads images from separate folders for positive (cracked) and negative (non-cracked) samples.
Preprocesses images by resizing them to a fixed size (64x64) and normalizing pixel values.
Data Splitting:

Splits the preprocessed data into training and testing sets using an 80-20 split.
Model Building:

Constructs a simple Convolutional Neural Network (CNN) model using TensorFlow and Keras.
Compiles the model with the Adam optimizer and binary crossentropy loss function.
Model Training:

Trains the model on the training data for 10 epochs with a batch size of 32.
Model Evaluation:

Evaluates the trained model's performance on the test data, providing the test accuracy.




Model Code:

The model code demonstrates how to use the trained crack detection model to classify new images.

Image Loading:

Utilizes OpenCV to load and preprocess an image selected by the user.
Model Loading:

Loads the pre-trained crack detection model.
Prediction:

Classifies the selected image using the loaded model.
Displays whether the image contains a crack (positive class) or not (negative class) based on the prediction probability threshold of 0.5.
These two parts work together: the trainer code prepares and trains the model, while the model code applies the trained model to new images for crack detection.
