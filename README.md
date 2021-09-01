# Machine learning Codes.

This repository holds the code for  different machine learning techniques learned/revisited with Siddharth Dhar (dharsiddharth7).

## Setup 

1) Clone the Repository.
2) Make a conda or pip virtual environment. 
3) In the terminal with the virtual environment activated run "pip install -r requirements.txt"
4) Start the jupyter server.
5) For a particular notebook dataset links are provided (in table below) if the code does not download the dataset automatically. Download those datasets and put it in "./Datasets/{Dataset_name}/" ( Replace the space with _ in dataset name)
6) Run the code in the notebook.

Please note: I am using a conda environment on an Apple M1 chip based computer. I do not use the GPU. Some parts of code might need some change to run with GPU. I will try to make the notebooks machine independent but not providing any guarantee of the same.

## Current status of planned work:

| Topic/Technique   | Dataset | Jupyter Notebook File | 
|-------|--------|-------|
| Linear Regression | [Linear Regression](https://www.kaggle.com/andonians/random-linear-regression) | [Linear_Regrression_Linear_Regrression.ipynb](Jupyter_Notebooks/Linear_Regrression_Linear_Regrression.ipynb)|
| Multiple Linear Regression | [Startup](https://www.kaggle.com/karthickveerakumar/startup-logistic-regression) | [Startup_Multiple_Linear_Regression.ipynb](Jupyter_Notebooks/Startup_Multiple_Linear_Regression.ipynb)|
| Multiple Linear Regression | [Car Price Prediction](https://www.kaggle.com/hellbuoy/car-price-prediction) | <span style="color:orange">Next</span> |
| Linear Classification | [Fish Market](https://www.kaggle.com/aungpyaeap/fish-market) | [Fish_Market_Linear_Classification.ipynb](Jupyter_Notebooks/Fish_Market_Linear_Classification.ipynb)|
| Convolutional Neural Network (CNN) | MNIST | [MNIST_Convolutional_Neural_Networks.ipynb](Jupyter_Notebooks/MNIST_Convolutional_Neural_Networks.ipynb)|
| Convolutional Neural Network (CNN) | CIFAR10 | [CIFAR10_Convolutional_Neural_Networks.ipynb](Jupyter_Notebooks/CIFAR10_Convolutional_Neural_Networks.ipynb)|
| Polynomial Regression | | <span style="color:Red">Not Started</span> |
| Support Vector Regression (SVR) | | <span style="color:Red">Not Started</span> |
| Decision Tree Reggresion (DTR) | | <span style="color:Red">Not Started</span> |
| Random Forest Regression | | <span style="color:Red">Not Started</span> |
| Logistic Regression | | <span style="color:Red">Not Started</span> |
| K nearest neighbors | | <span style="color:Red">Not Started</span> |
| Support Vector Machine | | <span style="color:Red">Not Started</span> |
| Kernel SVM | | <span style="color:Red">Not Started</span> |
| Decision Tree Classification | | <span style="color:Red">Not Started</span> |
| Random Forest Classification | | <span style="color:Red">Not Started</span> |
| k Means Clustering | | <span style="color:Red">Not Started</span> |
| hierarchical Clustering | | <span style="color:Red">Not Started</span> |
| Apriori | | <span style="color:Red">Not Started</span> |
| Eclat | | <span style="color:Red">Not Started</span> |
| Reinforced Learning | | <span style="color:Red">Not Started</span> |
| Deep Learning | | <span style="color:Red">Not Started</span> |

## My notes:

1) df.isnull().sum() is used to find nulls in dataset.
2) For linear regression number of layers required around sqrt(number of features). 
3) For CNN you can use this formula [(W-K+2P)/S]+1
      W is the input volume - in your case 128
      K is the Kernel size - in your case 5
      P is the padding - in your case O i believe
      S is the stride - which you have not provided.
   you can also use (W - (k-1)/2) for one max_pool
4) For CNN input and output channels are 1 or 3, 1 is greyscale and 3 is rgb color. 
5) Tensor need the image in a particular format of NCHW where N is number of images being passed, C is channel (1 or 3), h is height of image and w is the width of the image. 
6) matplotlib takes image in the format of HWC. point 4 for what each stand for.

