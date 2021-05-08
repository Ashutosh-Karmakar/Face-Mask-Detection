![Screenshot (118)](https://user-images.githubusercontent.com/60296760/117527194-1dc3a300-af7f-11eb-8a9b-576a11a92033.png)
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
 <li>adding it ti <b>images = []</b> list </li>
 <li>corresponding lable are added to <b>label = []</b></li>
 <li>then I convert it to one hot encoding i.e [0,1] for mask and [1,0] to mask </li>
 <li>then I are using sequential model of keras to and only adding layes </li>
 </ul>
 
![Uploading Screenshot (118).png…]()

 
 <ul>
 <li>here I have created a model with <b>4</b> layers first 64 nodes then 128 and then 64 and last layer is 2 nodes for <b>mask</b> and <b>no mask</b> </li>
 <li>then I am traing the model with 60 epoachs </li>
 </ul>
 

 
 <ul>
 <li>then I am saving it</li>
 <li>then i load it by <b>model = load_model("< name >.h5")</b></li>
 <li>then using opencv to detect the face area using <b>haarcascade_frontalface_default.xml</b></li>
 <li>then we take that frame numpy array and sending it for prediction</li>
 <li>it returns the result then we give 1 to max value in result</li>
 <li>and then display the image by drawing the rectangle and text on it</li>
</ul>


## we can also detect still images in the same way



