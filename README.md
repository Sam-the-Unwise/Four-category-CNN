# Four Category Classifying CNN

This is a Convolutional Nueral Network (CNN) project that was built with the hopes of it being able to successfully differentiate between four different animals just based on pictures. These animals are: cat, dog, koala, and duck. The CNN was built using Keras with Tensorflow and contains two main files built by us: testing.py and executeTest.py. This CNN was created as a base model for a future project, which can be found at (https://github.com/Sam-the-Unwise/Caribou-Classification-AI) and thus was developed underneath that repository. If you wish to see process of our development, please go to that repository.

## Getting Started

<i> Please note, most of this code was downloaded from or created by the Python library Keras and we are not claiming any of it to be our own work. The only things that were created by us are the testing.py and executeTest.py files </i>

The following instructions are meant to help you understand the code in broad detail. For a more detailed explanation, please see the file notes_on_training_CNN.py, which has extensive comments that explain the code. Also please sea

### Prerequisites

```
python
```
Install
```
pip install  tensorflow, Keras, numpy, os, math, random
```
<i> please note that for our model we had to download specific things that needed to be added to the Keras library but as many of these were different for our individual machines, I have chosen to leave them off </i>

### trainingCNN.py

This script contains all the methods necessary for training the AI. This script creates the CNN model and then trains the CNN based on the images that have been placed in the 'Dataset/training' folder. While training the CNN, the program will also test the CNN for accuracy using images from the 'Dataset/test' folder, which will allow the program to display an accuracy of how well the model is predicting. The data of the model is then saved underneath the folder 'models' in the files 'model.h5' and 'weights.h5'.

<i> Note that with our current set up of 25 epochs, 3000 training batch size, and 100 test batch size, the model was roughly at 78% accuracy. </i>

### testingCNN.py

This script contains all the necessary methods for testing our AI against desired photoes. The program accesses the folder 'Dataset/single_prediction' and tests each of the pictures in the folder against the saved model. The program will then output a prediction of what it thinks the picture is of (between the choices of cat, dog, duck, and koala).

### Team notes

Our reasoning behind choosing these animals is because cats, dogs, and koalas look very similar while ducks look very different. We chose to use these because, while testing the model, we could see specifically if it was giving the wrong prediction because the animals simply looked similar or because the model hadn't been trained correctly (should that mean too small of a data set, not enough epochs, a small training batch size, etc.)

We left the model at 78% accuracy for now because of the sole reason that this current model takes about 12 hours to run on our computers, but the model can indeed be made to be accurate further. This will be a continued project by us as we attempt to see how accurate we can make our model.


# Authors

* **Samantha Muellner** - [GitHub](https://github.com/Sam-the-Unwise)

* **Keenan Swanson** - [GitHub](https://github.com/Keenanks)

## Acknowledgments

* **Katie Orndah, Ecoinformatics PhD. Student** - *Client*
