# End-to-end Multi-Class Dog Breed Classfication

### This project is a classification problem that involves the classification of dogs by their breeds, using Tensorflow 

### It makes use of transfer learning model to carry out its classification.

### The steps carried out in this project are:

1. The problem is defined

2. The data was gotten from: https://www.kaggle.com/c/dog-breed-identification

3. the metrics for evaluation is defined and the features of the data studied

4. the workplace is made ready by importing `Tensorflow 2.x` ,`Tensorflow Hub`, `numpy` and making use of a _GPU_ to speed up 
   computations 

5. exploratory data analysis _EDA_ is done on the data: get images and their labels, convert labels to array using 
   `numpy`, get unique labels, turn labels to boolean.

6. create a validation set from the training set
   
7. from `sklearn.model_sleection` import `train_test_split`
 
8. define a function that process images; turn images to tensors `tf.image.decode_jpeg(image,channels=3)` with 
   three color channels, normalize and resize images
   
9. define another function that turns images to batches

10. create training and validation batches

11. train your model: the URL of the model we want to use from TensorFlow 
    Hub: https://tfhub.dev/google/imagenet/mobilenet_v2_130_224/classification/5

12. create call backs to check and save the training progress and also stop training early if model is not improving

13. train model with subset of data , make predictions using unbatchified validation set, before training model on 
    full data
    
14. save model and make predictions on processed test data


