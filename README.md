# bacteria-classification

Welcome to our GitHub repository! This project is focused on developing a program that analyzes microscope images of bacteria to distinguish between their normal (control) state and their acid state. The program aims to identify differences between the two states and aid in bacterial research.

## Dataset Description

Our dataset consists of two folders:

1. *control:* This folder contains images of bacteria in their normal (control) state.

2. *acid:* This folder contains images of bacteria in their acid state.

Due to data privacy and restrictions, we cannot publish the dataset, but you can find example images of both control and acid states in the file `perform_images_before_and_after_changes`.

## File and Folder Descriptions

1. *convert_data_to_RGB:* The images originally arrived in mode I, and in this file, we convert them to the appropriate mode - RGB.

2. *perform_images_before_and_after_changes:* This file showcases examples of images before and after the conversion to RGB. It gives an insight into the changes made to the images during the process.

3. *build_new_split_data:* With a dataset of 7200 images in a 1:1 ratio between normal and acid states, we split them into three folders: train, test, and validation, while preserving the original ratios.

4. *try_hyperparameter_tuning:* In this file, we perform hyperparameter optimization to find the best parameters for learning rate, dropout, and dense layer size. This optimization is based on the DenseNet121 model.

5. *final_model:* This file contains the ultimate model, which includes the base model obtained from hyperparameter optimization. After training, we were able to achieve an accuracy close to 1, indicating highly accurate results.

## Reproducing the Results

As we cannot share the dataset, reproducing the exact results might not be possible. However, you can follow the general approach outlined below:

1. Convert Data: Ensure your microscope images are in RGB mode to work correctly with the program.

2. Data Preparation: Organize your images into "control" and "acid" folders, each representing the different states of the bacteria.

3. Data Split: If you have a similar dataset, divide it into training, testing, and validation sets, preserving the 1:1 ratio between normal and acid states.

4. Hyperparameter Tuning: Experiment with hyperparameter tuning to optimize the learning rate, dropout, and dense layer size for the DenseNet121 model or the model of your choice.

5. Model Training: Use the optimized model to train on your prepared dataset.

# **Links to the models:**
best model:
https://drive.google.com/file/d/12KATh7IlV_XHtjgzzxaJBRNeDCCwipYu/view?usp=sharing

model before fine tuning:
https://drive.google.com/file/d/1jTiNs_KPDdsFL8vcqEO_5G82oeay-tkK/view?usp=sharing

