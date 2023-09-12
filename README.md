# Fine-tuning Real-ESRGAN on Chest X-Ray Images

This project involves fine-tuning the Real-ESRGAN model (originally developed by Xinntao) on a Kaggle dataset of chest X-ray images. The dataset includes both normal and pneumonia X-ray images.

## Table of Contents
1. Introduction
2. Installation
3. Dataset
4. Usage
5. Results


## Introduction
This project aims to apply the power of Real-ESRGAN, a state-of-the-art super-resolution model, to the medical imaging domain. We are specifically focusing on chest X-ray images, both normal and those indicating pneumonia, sourced from a Kaggle dataset.

## Installation
To set up this project on your local machine, follow these steps:
1. Clone this repository: `git clone https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia.git`
2. Navigate into the cloned repository: `cd Finetuning_Real-ESRGAN_Pneumonia`
3. Install the necessary dependencies: Python >= 3.7 (Recommend to use Anaconda or Miniconda), PyTorch >= 1.7

## Dataset
The dataset used in this project is a collection of chest X-ray images, both normal and those indicating pneumonia, sourced from Kaggle. You can download it from [this link](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia). 
Note: The dataset has already been loaded onto the folder dataset > pneumonia > HDtrain

## Usage
To fine-tune the Real-ESRGAN model on the chest X-ray images, follow these steps:

1. Open notebook:  **FinetuneReal-ESRGAN.ipynb** 
2. Follow through notebook to see the process of how the data was finetuned
   
   a. Preprocessing of data
   
   b. Finetuning data
   
   c. Inference


## Results
(Here you can discuss the results you've achieved so far. If possible, include images or charts to illustrate these results.)



