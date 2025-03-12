# Animals-10 dataset
For this project, I worked with the Animals-10 dataset, which contains images of 10 different animal classes. The goal was to prepare the dataset for deep learning, ensuring proper structure, preprocessing, and analysis before training a model.

1. Check the directory structure (folders)
   
   The dataset originally had class names in Italian, but I renamed them to English using a dictionary (copied from translate.py that was in the folder with images) and os.rename().
2. Understand the file format
   
   Since datasets.ImageFolder worked fine, I confirmed that the dataset consists of image files (JPEG). But also checked it manually before.
3. Create a histogram to show the number of images per class
   
   It turned out that the dataset was quite unbalanced. Some classes contained more than 4,000 examples, while others contained less than 1,500.
4. Split the dataset into training, validation, and test sets
   
   Train set: 72% of the total dataset
   
   Validation set: 8% of the total dataset
  
   Test set: 20% of the total dataset
  
7. Convert images into tensors + Apply data augmentation
   
   To prepare the dataset for deep learning, I applied a series of transformations. First, all images were resized to 224×224 pixels for consistency. It's important to note that data augmentation parameters are different for train (and validation) and test subsets.
8. Denormalization
    
   Since normalization shifts pixel values, I implemented a function that reverses normalization. This allows proper visualization of images.
9. Visualize some examples from different classes
    
   I implemented show_images() to display a grid of sample images from the training, validation, and test sets. This helped verify that the dataset was correctly loaded and transformed.
10. Create DataLoaders for training and testing
