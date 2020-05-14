# Dog Breed Classification
* This project was a part of Udacity Deep Learning Nano Degree.
* Built a Convolution Neural Network using Pytorch to predict the breed of the given image.
* Used the dataset provided by Udacity
    * [Dogs Images](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip). This folder contains 133 Folders, each corresponding to a different dog breed.
    * [Humans Images](http://vis-www.cs.umass.edu/lfw/lfw.tgz)
* The main goal of this project is to finally create a function that takes an image as input and do the following
    * Given an image of a dog, your algorithm will identify an estimate of the canine’s breed
    * If supplied an image of a human, the code will identify the resembling dog breed.

## Requirements
* If you don't have python installed on your machine download it from [here](https://www.python.org/ftp/python/3.8.2/python-3.8.2.exe)
* Then install pip on your machine by downloading this [get-pip.py](https://bootstrap.pypa.io/get-pip.py) and from the downloads directory and  run ```python get-pip.py```
* To start working on the project run the following command after cloning the repository.
```
pip install -r requirements.txt
```
* I suppose Anaconda is already installed in the machine. Then run the following command
```
conda install pytorch torchvision -c pytorch
```

This would install all the requirements.
## Output
* The dataset contains images of dogs of 133 different Breeds
* Did some preprocessing on the data using **PyTorch Transforms**
* To identify whether an Image is a human or not used **Open CV**'s Face Detector.
* To identify whether an Image is a dog or not applied Transfer Learning using **VGG 16 Model** and changed the classifier for our needs.
* To identify the breed of a dog
    * First defined a Convolution Neural Network. The accuracy was low.
    * So again applied Transfer Learning using **VGG 16 Model** which is a Deep Convolutional Network and updated the classifier of the model with 133 outputs each for a different dog breed.
* For Further Information see the [notebook](https://github.com/saisrirammortha/Dog-Breed-Classifier/blob/master/dog_app.ipynb).
* The output of some instances of function are given below.
![Output Image](https://github.com/saisrirammortha/Dog-Breed-Classifier/blob/master/output.png)



