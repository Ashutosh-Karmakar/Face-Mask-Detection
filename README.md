#Face Mask Detection using KERAS
####This is my python lab project for my college in this i have used keras a machine learning and deep learning package made by google this is a part of tensorflow
In this project I am using a dataset from kaggle containing two folders one mask and another without mask which contains the images of people with **mask** and **without mask** and also i have added some of my images also

##How it works??

Here we are taking the image of size 112 * 112 
converting it to gray scale 
then to pixels
then to numpy array 
adding it ti **images = []** list
corresponding lable are added to **label = []**
then I convert it to one hot encoding i.e [0,1] for mask and [1,0] to mask
then I are using sequential model of keras to and only adding layes

image 

here I have created a model with **4** layers first 64 nodes then 128 and then 64 and last layer is 2 nodes for **mask** and **no mask**

image

then I am traing the model with 60 epoachs

image

then I am saving it
then i load it by **model = load_model("name.h5")**
then using opencv to detect the face area using **haarcascade_frontalface_default.xml**
then we take that frame numpy array and sending it for prediction
it returns the result then we give 1 to max value in result
and then display the image by drawing the rectangle and text on it


we can also detect still images in the same way


