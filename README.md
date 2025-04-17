# Animals-10 dataset
https://www.kaggle.com/datasets/alessiocorrado99/animals10/data

For this project, I worked with the Animals-10 dataset, which contains images of 10 different animal classes. The goal was to prepare the dataset for deep learning, ensuring proper structure, preprocessing, and analysis before training a model.


Technical requirements: using Kaggle's GPU T4 x2. 

Main technologies: PyTorch (torch, torchvision) for dataset handling, transformations, and deep learning model implementation.
Matplotlib & NumPy for data visualization and numerical operations.

The dataset has more than 26,000 images, which are divided into 10 classes. The classes are quite unbalanced, which is a serious disadvantage.
Split: training - 70%, val - 10%, test - 20%.

1. animal10-preprocessing.ipynb - a notebook with data analysis.

2. animals10-cnn.ipynb - a notebook with my own basic CNN model. 
Accuracy: 0.7368; F1 Score (weighted): 0.7352

3. animal10-advanced-cnn.ipynb - a notebook with an advanced CNN model. Accuracy: 0.8877;
F1 Score (weighted): 0.8873

4. animal10-resnet.ipynb - a notebook with Transfer learning & Fine-tuning the ResNet model. Accuracy: 0.9799; 
F1 Score (weighted): 0.9799


Please be sure to look for more details in the notebooks :D
