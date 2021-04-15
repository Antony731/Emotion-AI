# EMOTION AI - END TO END MACHINE LEARNING PROJECT
* Artificial Emotional Intelligence or Emotion AI is a branch of AI thatallow computers to understand human non-verbal cues such as body language and facial expressions. 
* The aim of this project is to classify people’s emotions based on their face images.
* We have collected more than 20000 facial images, with their associated facial expression labels and around 2000 images with their facial key-point annotations.

Data Source: https://www.kaggle.com/c/facial-keypoints-detection/data

# PART 1. KEY FACIAL POINTS DETECTION
* In part #1, we will create a deep learning model based on Convolutional Neural Network and Residual Blocks to predict facial key-points.
* The dataset consists of x and y coordinates of 15 facial key points.
* Input Images are 96 x 96 pixels.
* Images consist of only one color channel (gray-scale images)

# PART 2. FACIAL EXPRESSION (EMOTION) DETECTION
* The second model will classify people’s emotion.
* Data contains images that belong to 5 categories:
  * 0 = Angry
  * 1 = Disgust
  * 2 = Sad
  * 3 = Happy
  * 4 = Surprise
# MODEL DEPLOYMENT USING TENSORFLOW SERVING
* We want to integrate our trained Tensorflow model into a web app and deploy the model in production level environment.
* The following objective can be obtained using TensorFlow Serving. TensorFlow Serving is a high-performance serving system for machine learning models, designed for production environments.
* With the help of TensorFlow Serving, we can easily deploy new algorithms to make predictions.
* In-order to serve the trained model using TensorFlow Serving, we need to save the model in the format that is suitable for serving using TensorFlow Serving.
* The model will have a version number and will be saved in a structured directory.
* After the model is saved, we can now use TensorFlow Serving to start making inference requests using a specific version of our trained model
"servable".
# MAKING REQUEST IN TENSORFLOW SERVING
* In-order to make prediction using TensorFlow Serving, we need to pass the inference requests (image data) as a JSON object.
* Then, we use python requests library to make a post request to the deployed model, by passing in the JSON object containing inference requests (image data).
* Finally, we get the prediction from the post request made to the deployed model and then use argmax function to find the predicted class. 
