# STA2453_Project

This is the code for my STA2453 course project "CNN Classifier for Zooplankton Data". This repository contains two Jupyter notebooks: `Zooplankton_EDA.ipynb` is for generating images for exploratory data analysis (EDA) and `Zooplankton_model.ipynb` is for the convolutional neural network (CNN) models. 

This model takes a full TIFF image, along with its respective overlap.csv featured data as input to generate a probabilistic prediction for each of the seven zooplankton classes. The test accuracy of the final model is 85.11% with the following confusion matrix. 

![alt text]([https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png](https://github.com/CSG-JOS/STA2453_Project/blob/main/figures/confusion_matrix_full_model.png) "full_model_CM")

Moreover, ablation study is done to verify the effects of image and featured data to the model. The model trained using only TIFF images yields 78.3% test accuracy and the model trained using shape-related featured data from overlap.csv files yields 85.21$ test accuracy. The confusion matrices of these two models are as follows: 

![alt text]([[https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png](https://github.com/CSG-JOS/STA2453_Project/blob/main/figures/confusion_matrix_full_model.png](https://github.com/CSG-JOS/STA2453_Project/blob/main/figures/confusion_matrix_ablation.png)) "ablation_study_CM")

Before running either notebook on a local device, download the zooplankton dataset. store them in the same format as in the `example_data` folder, and then change the `dir` variable in the notebook to that directory. 
