# Face Mask Detection using KERAS
 Markup : - Bullet list
              - Nested bullet
                  - Sub-nested bullet etc
          - Bullet list item 2 
# Face Mask Detection using KERAS
#### This is my python lab project for my college in this i have used keras a machine learning and deep learning package made by google this is a part of tensorflow
In this project I am using a dataset from kaggle containing two folders one mask and another without mask which contains the images of people with **mask** and **without mask** and also i have added some of my images also

***

## How it works??
<ul>
 <li>Here we are taking the image of size 112 * 112 </li>
 <li>converting it to gray scale </li>
 <li>then to pixels</li>
 <li>then to numpy array  </li>
 <li>adding it ti **images = []** list </li>
 <li>corresponding lable are added to **label = []**</li>
 <li>then I convert it to one hot encoding i.e [0,1] for mask and [1,0] to mask </li>
 <li>then I are using sequential model of keras to and only adding layes </li>
 <li>image </li>
 <li>here I have created a model with **4** layers first 64 nodes then 128 and then 64 and last layer is 2 nodes for **mask** and **no mask** </li>
 <li>then I am traing the model with 60 epoachs </li>
 <li>Image</li>
 <li>then I am saving it</li>
 <li>then i load it by **model = load_model("name.h5")**</li>
 <li>then using opencv to detect the face area using **haarcascade_frontalface_default.xml**</li>
 <li>then we take that frame numpy array and sending it for prediction</li>
 <li>it returns the result then we give 1 to max value in result</li>
 <li>and then display the image by drawing the rectangle and text on it</li>

</ul>


## we can also detect still images in the same way

