[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

This is Convolutional Neural Networks (CNN) project, part of the deep learning nanodegree prvided by Udacity! 
In this project, I built a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, the implemented algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

In this project, I explor some state-of-the-art CNN models for classification and localization, I used a series of models designed to perform various tasks in a data processing pipeline such as:

1. __face detetcion__ using openCV pre-trained face detectors.
2. __Dog detetction__ using  VGG-16 model, which is a pretrained model on ImageNet, a very large, very popular dataset used for image classification and other vision tasks.
3. __CNN model for dog breeds detection__. This is a CNN model desigend from scratch to identify the dog breed. It will classify the dog image into one of 133 possible breeds (train]\test data are available online,please check the instruction section)
4. __CNN to Classify Dog Breeds (using Transfer Learning)__ I used transfer learning to create a CNN that can identify dog breed from images (VGG16 model)





### Instructions

1. Clone the repository and navigate to the downloaded folder.
	
	```	
		git clone https://github.com/udacity/deep-learning-v2-pytorch.git
		cd deep-learning-v2-pytorch/project-dog-classification
	```
	
2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dog_images`.  The `dog_images/` folder should contain 133 folders, each corresponding to a different dog breed.
3. Download the [human dataset](http://vis-www.cs.umass.edu/lfw/lfw.tgz).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 
4. Make sure you have already installed the necessary Python packages according to the requirements.txt file
5. Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
	
	```
		jupyter notebook dog_app.ipynb
	```

## (Optionally) Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen CNN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you can spin up an instance of your own:

#### Amazon Web Services

You can use Amazon Web Services to launch an EC2 GPU instance. (This costs money, but enrolled students should see a coupon code in their student `resources`.)

## Evaluation

The project has been reviewed by a Udacity reviewer against the CNN project rubric. check the PDF reviwe file if you want to read some suggested points for poissible improvments.

