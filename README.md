# Deep Learning Project – ResNet18 on LC25000 Dataset

This project was carried out during my Erasmus semester while attending the Deep Learning Master’s course.  
It may also serve as the foundation for my upcoming bachelor thesis.  

## Overview  
The project focuses on **image classification using ResNet18**.  
- The ResNet18 model was taken from PyTorch.  
- **Transfer learning** was applied, meaning only the last layer was trained.  
- Training was done for a small number of epochs, since this is just a **simplified prototype** and a starting point for a larger project.  

## Dataset – LC25000  
The dataset used is **LC25000**, a publicly available medical dataset with labeled images of lung and colon tissues.  
Because of its size, I provide a link here: https://github.com/tampapath/lung_colon_image_set

### Dataset labels:  
- `colon_aca`: colon adenocarcinoma (cancer)  
- `colon_n`: normal colon tissue  
- `lung_aca`: lung adenocarcinoma (cancer)  
- `lung_n`: normal lung tissue  
- `lung_scc`: lung squamous cell carcinoma (cancer)  

## Preprocessing  
- **Normalization** and **augmentation** were applied (resizing, flipping, rotation).  
- The dataset was not originally split into training and validation sets, so a script `organize_data` was created to:  
  - split the data,  
  - store it on Google Drive,  
  - and prepare it for training in Google Colab.  

## Training  
- **Loss function**: Cross Entropy Loss  
- **Optimizer**: Adam  
- **Training/Validation**: performed on the processed dataset in Colab  

## Notes  
This project is just a **schema/prototype** for a larger project.  
The training was intentionally short and limited to illustrate the workflow.  



