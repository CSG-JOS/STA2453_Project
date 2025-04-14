# STA2453_Project

This is the code for my STA2453 course project "CNN Classifier for Zooplankton Data". This repository contains two Jupyter notebooks: `Zooplankton_EDA.ipynb` is for generating images for exploratory data analysis (EDA) and `Zooplankton_model.ipynb` is for the convolutional neural network (CNN) models. 

This model takes a full TIFF image, along with its respective overlap.csv featured data as input to generate a probabilistic prediction for each of the seven zooplankton classes. The test accuracy of the final model is 85.11% with the following confusion matrix. 

Moreover, ablation study is done to verify the effects of image and featured data to the model. The model trained using only TIFF images yields 78.3% test accuracy and the model trained using shape-related featured data from overlap.csv files yields 85.21$ test accuracy. The confusion matrices of these two models are as follows: 

Before running either notebook on a local device, download the zooplankton dataset. store them in the same format as in the `example_data` folder, and then change the `dir` variable in the notebook to that directory. 
