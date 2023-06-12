# Automated-Face-Detection
Automated Face Detection for Movie Streaming Application

Project Description:

In the domain of entertainment, Company X owns a movie application and repository that provides movie streaming services to millions of subscribers. To enhance the user experience, the company aims to automate the process of retrieving cast and crew information for each scene in a movie. When a user pauses the movie and clicks on the cast information button, the application should display details of the actors present in the scene. To achieve this, the company's in-house computer vision and multimedia experts need to develop a face detection system that can detect faces from screenshots of movie scenes.

The project's objective is to build an efficient face detection system using computer vision techniques. The dataset provided consists of images and corresponding masks for human faces. The data labeling has already been done, and the masks indicate the coordinates of the face regions in the images.

The project will be carried out in the following steps:

1. Import and Understand the Data:
   - Read and import the 'images.npy' file containing the images.
   - Split the data into features (X) and labels (Y), unifying the shape of all images.
   - Replace pixels within the masked area with 1 in the labels.
   - Split the data into training and test sets.

2. Model Building:
   - Design a face mask detection model using the MobileNet architecture with initial pre-trained non-trainable layers.
   - Add appropriate upsampling layers to imitate the U-net architecture.
   - Design a custom Dice Coefficient and Loss function.
   - Train and tune the model as required.
   - Evaluate the model's performance and provide insights.

3. Test Model Predictions:
   - Apply the trained model to predict masks on the test image with index 3 in the test dataset.
   - Visualize the predicted masks on the faces in the image.

By successfully developing the face detection system, Company X will be able to automate the process of extracting cast information from movie scenes. This will provide users with a convenient way to access details about the actors in each scene, enhancing their movie-watching experience.
