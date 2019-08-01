# CV-Handwritten-Digit-Recognition
It is done by training the classifier from MNIST database.
The training images and labels are downloaded and then extracted.
The extracted .idx3 files are converted to numpy arrays and then given as inputs to arrays labels and features.
After that we calculate HOG features for each image in dataset and save them in another numpy array.
Then  we create a linear SVM object. The Linear SVM that comes with sklearn can perform multi-class classification.
When the training finishes, we will save the classifier in a file named digits_cls.pkl
# Testing
Now we give our input image,grayscale it, apply Gaussian filter,convert it to binary using threshold value of 90.
Then we find contours and draw bounding square for each contour. Then we resize it to 28x28 and dilate it.
Then we calculate hog features and predict the digit using classifier.


# For reference use 
http://hanzratech.in/2015/02/24/handwritten-digit-recognition-using-opencv-sklearn-and-python.html
