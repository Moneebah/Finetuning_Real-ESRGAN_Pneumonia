# Fine-tuning Real-ESRGAN on Chest X-Ray Images

This project involves fine-tuning the Real-ESRGAN model (originally developed by Xinntao) on a Kaggle dataset of chest X-ray images. The dataset includes both normal and pneumonia X-ray images. <br>
Currently, the Real-ESRGAN model is not suited for xray images whereby the images lose the details (necessary in case of detecting pneumonia and other diseases) and it seems that the images have just been over sharpened. <br>
To account for this, this model was finetuned to better fit chest xray data 

![image](https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia/assets/129015993/99c9f42a-a55a-465b-b107-aaced42b59c1)
![image](https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia/assets/129015993/bf514d94-5b14-44fc-b6cb-8db720ec2bc5)



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
2. Follow through notebook to see the process of how the data was finetuned <br>
   a. Preprocessing of data <br>
      Dataset was scaled into three different sizes (0.5, 1/3, 0.18)<br>
      Dataset was cropped into subimages <br>
      Meta information was created <br>
   b. Finetuning data <br>
      Changes in the configuration file (see notebook) <br>
      Trained for 3,500 interations <br>
   c. Inference
      Model inference performed on original and finetuned model


## Results
![image](https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia/assets/129015993/89690e83-2a88-4b87-8309-904aded8083b)
![image](https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia/assets/129015993/89ad78f0-8df0-44da-a97a-103d05f8fd8f)
![image](https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia/assets/129015993/986d297d-3e6e-40d0-9130-87335a9eea94)
![image](https://github.com/Moneebah/Finetuning_Real-ESRGAN_Pneumonia/assets/129015993/1d2b7b82-afb0-4ada-b983-73ff9062e117)







