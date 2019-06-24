# Sign-Language-Digits-Detector


<p align="center"> Kaggel problem/data =https://www.kaggle.com/ardamavi/sign-language-digits-dataset.
    <br> 
</p>


## 🧐 About <a name = "about"></a>
our scoup for this project to classify signs with acc. higher than 85%

sign language digits (0-9)

[avilable data](https://www.kaggle.com/ardamavi/sign-language-digits-dataset)

Image size: 100x100 Color space: RGB


### Prerequisites
Python==3.0 or higher.
Keras==2.2.2.
tensorflow==1.10.0.
numpy==1.14.3.
scikit-learn==0.19.1.
opencv==3.42.
recommend to use anaconda3 for dependency installation.

### Installing
recommend to follow the instarction to install [anaconda3](https://www.anaconda.com/distribution/).
After installin run anaconda then create environment and install Keras & tensorflow,OpenCV


### Main Steps:

1. Read data
read data using OpenCV
2. preprocessing
thershold Trunc
make sure to rescale all images to 100*100

3. convert color space to grey scale
4. save data as npy
5. use keras (TF-based) to create model (CNN)
input shape = 100*100*1 (grey scale)
2Conv2D (relu),MaxPooling2D,Dropout,Flatten,Dense(relu),Dropout,Dense(softmax may make aconflect so use tf.nn.softmax)

6. Train
you mas use image genrator to alter the images befor training
epoch =20 , batch size =16
9. Predicte and Evaluate the Model
Accuracy ~= 93-96 %
