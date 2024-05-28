# flame-ai-challenge

## Description

This repository contains our submission to the [ML Challenge](https://www.kaggle.com/competitions/2023-flame-ai-challenge/overview) organized by the [Stanford FLAME AI 2023 Workshop](https://flame-ai-workshop.github.io/).  
The challenge's objective is to perform super-resolution on low-resolution 2D flowfield images to reconstruct high-resolution versions of these flowfields.  
<img src="./images/illustration.png" alt="Illustration" width="400"/>


## Requirements
This code is written in python, and needs pytorch and torchvision to run. It is optimized for GPU usage.


## Installation
- Clone this repository
- Copy the [data](https://www.kaggle.com/competitions/2023-flame-ai-challenge/data) from the challenge to the `data` folder. The folder structure should be as follows:
```
data
├──dataset
    ├── train.csv
    ├── test.csv
    ├── val.csv
    ├── flowfields
    │   ├── ...
```
- Download the models checkpoints into the `checkpoints` folder. The folder structure should be as follows:
```
checkpoints
├── model_1.pth
├── ...
```


## Usage
- Launch jupyter lab
- Open `loading_model.ipynb`


## Results
The model achieves a L2 loss of :
- 0.00553 on the private test set
- 0.00462 on the validation set

The best individual model `vxyhe45d` achieves a L2 loss of:
- 0.00600 on the private test set.
- 0.00478 on the validation set


## Team Members
- Thomas X Wang, ISIR, Sorbonne Université
- Louis Serrano, ISIR, Sorbonne Université


## Acknowledgements
This code is based on [Super-Resolution Neural Operator](https://github.com/2y7c3/Super-Resolution-Neural-Operator)
