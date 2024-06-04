**DAN Unilateral Model Trained on CWRU Dataset**

This repository contains the code for a Dan unilateral model trained on the CWRU dataset. The model is a convolutional neural network (CNN) that can be used to classify the health state of a bearing.
You can directly the file from the following [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RflxmpM7Iw9M0u6zPo8Ma5O-ZSHggejd?usp=sharing)

**Dataset**

The CWRU dataset is a collection of vibration data from bearings in different health states. The dataset is divided into four sets:

* **Set 1:** Normal bearings
* **Set 2:** Bearings with inner race faults
* **Set 3:** Bearings with outer race faults
* **Set 4:** Bearings with ball faults

**Fetching Dataset:**

1. Clone this repository to your local machine/Google Colab
2. Install the required libraries while on local machine. Google colab can easily handle most of them.
3. Download the CWRU dataset from the following website : https://www.kaggle.com/datasets/astrollama/cwru-case-western-reserve-university-dataset/data .
   The google colab automatically downloads the datatset. If there is some problem with the dataset then you can always download it and reupload it or run in local machine. 

**Model**

The Dan unilateral model is a CNN that consists of the following layers:

* **Input layer:** This layer takes a 1-dimensional array of vibration data as input.
* **Convolutional layer:** This layer applies a series of filters to the input data to extract features.
* **Dropout layer:** This layer randomly drops out a certain percentage of the neurons in the previous layer to prevent overfitting.
* **Fully connected layer:** This layer connects all of the neurons in the previous layer to the output layer.
* **Output layer:** This layer outputs the probability of each health state.

**Training**

The model was trained on the CWRU dataset using the following steps:

1. The data was divided into training and validation sets.
2. The model was compiled with the Adam optimizer and the categorical cross-entropy loss function.
3. The model was trained for 200 epochs.
4. The model was evaluated on the validation set.

**Results**

The model achieved an accuracy of 98.5% on the validation set. The following image shows the results during the training of the model.
![alt text](image.png)

**Usage**

The model can be used to classify the health state of a bearing by following these steps:

1. Load the vibration data from the bearing.
2. Preprocess the data by removing the mean and normalizing the data.
3. Pass the data through the model.
4. Get the output of the model, which is the probability of each health state.

**A YouTube tutorial is also available that elucidates the concepts employed in this model:**
