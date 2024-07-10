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
* Place raw data [file](https://drive.google.com/file/d/1i5MLRjzv1pu9IDysmENGG-W0eVh6wnPq/view?usp=drive_link) under the folder: 'data/raw/'
* Place processed data [file](https://drive.google.com/file/d/1Kig-1B7w3Hcjq-IJCfssf78Ls-0qwbtO/view?usp=drive_link) under the folder: 'data/processed/'
* Place train data [file](https://drive.google.com/file/d/1o0N9KLz9sAKzMfkDrlGpaiSA1lFpD-d3/view?usp=drive_link) under the folder: 'data/processed/'
* Place test data [file](https://drive.google.com/file/d/1dhd6OQyZuMHHvunuQYNzNYrZ3QcVtpP7/view?usp=drive_link) under the folder: 'data/processed/'
### Checkpoints
* Place model [file](https://drive.google.com/file/d/1QwSmrKSJ-QLk_y-9egVEDPNWDK0DSC1_/view?usp=drive_link) under the folder: 'models/'

## How to run?
* Prepare raw data by running notebooks/data_preparation.ipynb
* Predict bandgaps by running notebooks/bandgap_prediction.ipynb
## Publication
*The work has been published and you can find it at https://doi.org/10.1002/adts.202400190
