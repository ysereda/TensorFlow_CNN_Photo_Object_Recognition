# TensorFlow_CNN_Photo_Object_Recognition
End-to-end TensorFlow pipeline for building a multi-label image classification model, including recursive image collection, annotation, preprocessing, CNN training, evaluation, and prediction.
Stages:
* Collect images recursively from folders (I used my own collection of photos).
* Resize and preprocess images (original images with resolution 5184x3456 and 4608x3456 were downsized to 150x100 pixels).
* Create annotation tool (human labels; used OpenCV library for image loading, preprocessing and displaying. Number of recognized objects is 7).
* Save labels to CSV.
* Load dataset into TensorFlow.
* Train a multi-label CNN (25 epochs).
* Save the model.
* Predict on new images (the input is a downsized image, and the output is a vector of probabilities for each of the 7 tracked objects).
* Evaluate.
