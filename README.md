# FaceNet-for-face-recognition

This repository is a first time implementation of face recognition using FaceNet.

FaceNet is a neural networks that has a functions as calculating the Euclidean distance between the similar images. This is also called as a Siamese network.

This network uses a specific concept called Triplet loss for loss calculation.

I have referred the blog article listed on https://www.freecodecamp.org/news/making-your-own-face-recognition-system-29a8e728107c/

For implementation purposes we use libraries like keras, tensorflow, opencv. For sample models and weights for pre-trained weights we have used inception, acquired for David Sandberg's implementation techniques. Also, we use the utility files fr_utils.py and inception_blocks_v2.py. These files encodes images and compile the FaceNet network respectively.

We kept the image size to be 96x96 pixels with three channels RGB. Here we use Adam optimizer to optimize the loss generated using the Triplet loss. I am using two images for now for implementation purposes.

The embedding and distance for the images is been calculated. Post this we can use opencv to turn on the webcam to get the live video feed and use haar cascade xml file to detect faces and match the detected faces and calculate the distances to similarity of images.

The distances will be printed and same will be used to identify who is there in image.


## How to install
To install all the requirements for the project run

pip install -r requirements.txt


## How to run project

TO run the project use below command

python facenet.py

## P.S.

You can add your image in the directory './images', which results the webcam to identify and recognize your face
