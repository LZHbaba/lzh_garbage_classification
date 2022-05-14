# Garbage Classification
## Introduction

Use the prevalent models like DenseNet201, InceptionV4, MobileNetV3Large, SE-Nets as the backbone model,
Test those models with a G-FC complement architecture based on fine tuning and dataset `Garbage Classification`.
Choose the optimal backbone model to create the G-model with the G-FC complement architecture.
Use the ablation study to choose optimal model parameters, including `trainable layers`, `training epochs` in 
`freezed process` and `unfreezed process`, `patience` in `EarlyStopping` and `ReduceROnPlateau`.
Finally, use `Lable Smoothing Regularization` to take place the `Categorical Cross Entrophy` to improve the 
evaluation result.

## DataSet 
The `Garbage Classification` dataset comes form Kaggle, its link is:
https://www.kaggle.com/datasets/asdasdasasdas/garbage-classification

## Code file

1. [EfficientNets.ipynb](#EfficientNets.ipynb)
    * `EfficientNets.ipynb` is the code for realizing train process of the `EfficientNetB1`,`EfficientNetB2`,`EfficientNetB3`.
2. [InceptionResNetV2.ipynb](#InceptionResNetV2.ipynb)
    * `InceptionResNetV2.ipynb` is the code for training `InceptionV4`
3. [SE_ResNet152_20_last20_4_8.ipynb](#SE_ResNet152_20_last20_4_8.ipynb)
    * `SE_ResNet152_20_last20_4_8.ipynb` is the code for training `SE-Resnet152` and `SE-ResNet50` 
4. [mobileNetAll.ipynb](#mobileNetAll.ipynb)
    * `mobileNetAll.ipynb` is used to choose the optimized parameters.
5. [draw_pictures(parameters).ipynb](#draw_pictures(parameters).ipynb)
    * ` draw_pictures(parameters).ipynb` is the file for drawing `train loss`,`validation loss`,`train accuracy`,`validation accuracy`,`error difference` of all backbone models.
6. [final_presentation.ipynb](#final_presentation.ipynb)
    * `final_presentation.ipynb` is the code I used in oral presentation
    * The G-model downloads pretrained parameters (weights, bias) directly.
    * Connect with the anvil to create a interactive interface to display the performance of my G-model.
    * Show Histogram pictures and Confusion Matrix.

## Display
 Users can access the link to predict related types of garbage trash.
 
