# Mammography_On_Minimias

The goal of this project detect Breast Cancer on Mammograms using the Vision Transformer (ViT) architecture. The dataset used for this task is the MINIMias dataset, containing grayscale medical images. The project involves training a ViT model on this dataset and evaluating its performance through a 5-fold cross-validation approach.
## Details of Project Working:
- Dataset consists of 2 classes, Benign and Malignant. 
- We train a ViT model on the MiniMIAS dataset.
- Seperated a test set and train set (80/20)
- Apply a K-fold to train set, K = 5
- Apply data augmentation to training set as well ( using transform)
- train each fold on 25 epochs.
- used model: google/vit-base-patch16-224-in21k
- Best weights for the trained model are available at: https://drive.google.com/file/d/1zjJxWvaGiCZG7O8toKNPFJ8YuojfKwoU/view?usp=sharing
- can be imported in the testing cell

## Steps to run:
1. pip install torch torchvision transformers matplotlib scikit-learn
2. Run the notebook
3. Run the training cell to re-do training
4. Run the Testing cell to test the best model on the test set (Testing Cell is already run on trained model)
