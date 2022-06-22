# Identifying Entities in Healthcare Data - NLP

**Student:**  Jheser Guzman

## Introduction 

In this programming assignment I built a CNN model to detect melanoma in a pictures dataset.

This repository contains the following file required by the assignment:

* Jupyter Notebook file with the Data Preparation and Model Building to detect Melanoma.

## Methods Used

* Python
* Pandas
* Numpy
* Scikit-Learn
* Spicy

## Download and Setup

This project needs Jupyter Notebook with SciKit-Learn and Spacy libraries.

* For more details about the instalation in Anaconda, go to:  https://docs.anaconda.com/anaconda/install/index.html

### How to Run

You can download the source code cloning this repository using Git:

1. Open your favorite Terminal app (Unix, Linux or Macos), such as Terminal, Command, Console, iTerm2, so on.

2. Clone the repository

```
git clone https://github.com/dicotips/NER_Healthcare_Assignment.git
```

3. Open the ** *.ipynb** notebook file in Anaconda.

```
jupyter notebook Jheser_Guzman_CNN.ipynb
```

## Problem Statement

To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Final Conclusion

We observe successive improvement from Model 1 to Model 3 based on the Training and validation (test) data as you can see in:

* **Model 1:** Simple CNN Model | Accuracy: 0.9431 | Validation accuracy : 0.8306
* **Model 2:** CNN Model with Dropout | Accuracy: 0.9344 | Validation accuracy : 0.8639
* **Model 3:** CNN Model with Augmented Data, Dropout and Batch Normalization | Accuracy: 0.9632 | Validation accuracy : 0.8306

We see an increment in the Validation dataset using Aumented Data and managing DRopouts and Batch Normalization. The Accuracy of the Model 2 is the best one in this experiment, but since the neural network can optimize in a local optima, in a re-training we can get a better result. The model 3 is overfiging comparing against model 2. 

As conclusion, in this experiment I showed that the CNN Model with Droponts performs better than managing Augmented Data.

### Future Word
I can improved the accuracy in the further with proper hyper-parameter. I can setup different CNN Configuration, other chose of loss function, Optimizers and Layers to test if it improves the accuracy