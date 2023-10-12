# BandGap Prediction

## Introduction

## Environment Setup
We would recommend to use seperate conda environment for installing all the required packages , if it is not already installed on your system, you can install it by following their official installation [guide](https://docs.anaconda.com/free/anaconda/install/index.html). 
Once you install anaconda properly, follow the following steps to properly install all the required dependencies:
```
conda create -n mat_env python=3.10

conda activate mat_env

conda install jupyter

pip install -r requirements.txt
```
For data retrieval from materials project, data_preparation.ipynb also require a materials project API key which you can get by creating a account on [materials project](https://next-gen.materialsproject.org/api).
Once you have the API key, write it inside the 'example.env' file and rename the file to '.env'.

## Datasets and Pre-trained model checkpoints
You can either prepare data and train your own model or download the already prepared dataset files and model checkpoints.
### Datasets
* Place raw data [file](https://drive.google.com/drive/folders/1OkwNdpAzwk_nXBUd6IV4ujZ0eUEDwYYX?usp=sharing) under the folder: 'data/raw/'
* Place processed data [file](https://drive.google.com/drive/folders/1OkwNdpAzwk_nXBUd6IV4ujZ0eUEDwYYX?usp=sharing) under the folder: 'data/processed/'
### Checkpoints
* Place model [file](https://drive.google.com/drive/folders/1OkwNdpAzwk_nXBUd6IV4ujZ0eUEDwYYX?usp=sharing) under the folder: 'models/'

## How to run?
* Prepare raw data by running notebooks/data_preparation.ipynb
* Predict bandgaps by running notebooks/bandgap_prediction.ipynb