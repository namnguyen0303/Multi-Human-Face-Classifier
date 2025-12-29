# Multi-Human Face Classifier

## Project Summary
This project implements a **multi-human face classification system** using **transfer learning** with a pre-trained **ResNet18** model. The objective was to build, train, and evaluate a deep learning model capable of classifying face images belonging to multiple individuals.

The entire pipeline—from data preprocessing to model evaluation—was completed in a Jupyter Notebook environment.

---
## Dataset
https://drive.google.com/file/d/1q23xEeSfhe3famj7bgXc8tLNyuY040im/vie

## Model Info
- **Base Model:** ResNet18 pretrained on ImageNet with included pooling 
- **Modified:** Final FC layer replaced with num_classes outputs  
- **Optimizer:** Adam (lr = 1e-4)  
- **Loss:** CrossEntropyLoss  
- **Batch Size:** 16  
- **Epochs:** 5  

## What I Did
- Selected **ResNet18**, a pre-trained convolutional neural network, as the base model
- Modified the final fully connected layer to support **multi-class face classification**
- Implemented **data loading and preprocessing**, including resizing and normalization
- Applied **data augmentation** to improve generalization
- Trained the model using transfer learning
- Evaluated model performance on a held-out test dataset
- Visualized training and validation loss and accuracy

---

## What Was Completed
- ✔️ Successful implementation of transfer learning with ResNet18  
- ✔️ Multi-class face classification model trained and tested  
- ✔️ Training and testing datasets properly structured and loaded  
- ✔️ Model evaluation using accuracy metrics  
- ✔️ Training performance visualized through plots  
- ✔️ End-to-end deep learning pipeline fully functional  

---

## Results
- The trained model achieved **strong classification accuracy** across multiple face classes
- Training and validation loss curves show stable convergence
- The use of transfer learning significantly reduced training time while maintaining good performance
- The model was able to correctly distinguish between different individuals in the dataset

# Results
- **Final Accuracy:** 74 %  
- **Training Loss :** 0.198 
- **Precision:** 0.73 
- **Recall:** 0.74  
  The model was trained for 5 epochs using transfer learning on ResNet18, with Adam optimizer and CrossEntropyLoss.
---

## Live Demo
A Gradio-based web interface was implemented to demonstrate the model:
- Upload a face image
- View predicted identity
- Display top-5 predictions with confidence percentages

