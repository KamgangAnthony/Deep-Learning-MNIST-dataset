# DEEP LEARNING : MNIST DATASET

* The objective is to create an algorithm that can identify the written digit in an image.
This is a classification issue with 10 classes as there are only 10 numbers (0, 1, 2, 3, 4, 5, 6, 7, 8, 9).

* The dataset offers 70,000 handwritten digit pictures (28x28 pixels) (1 digit per image).

* Use deep learning to identify the digits that are written in the picture.

* The dataset is called MNIST and refers to handwritten digit recognition.

**Python Version:** 3.10.5

**Packages:** pandas, numpy, sklearn, matplotlib, tensorflow, tensorflow_datasets

**For Web Framework Requirements:** ```pip install -r requirements.txt```

I discovered the data was clean after importing it, so I:

* Separated the data into train and test sets.

* Scaled the data since doing so greatly increases accuracy

* Shuffled the data to enter batching so it does not confuse the stochastic gradient descent

* Adjusted the batch size that would be introduced into the deep learning model at a given moment.

* Developed a model with 10 outputs representing the numbers 0 through 9 and 784 inputs.

* Used 'relu' as the activation function in the hidden layers and 'softmax' in the output since we are dealing with multi-classification

The photos in the dataset are organized as follows:

![alt text](image.PNG "How the images in the dataset are")

The digits in each picture must then be recognized by the algorithm.

With a test accuracy of 97.28 percent, the model successfully categorized 9 out of every 10 photos. 