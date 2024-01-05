# Plant Doctor - Yellow Mosaic and Rust Disease Detection on Green Grams

## Overview
This project demonstrates the process of building a simple image classification model using PyTorch. The model is designed to classify plant diseases, with a focus on detecting yellow mosaic and rust diseases on green grams.

## Requirements
Before running the project, ensure you have the following dependencies installed:

- PyTorch
- torchvision
- Google Colab (if running on Colab)
- Matplotlib
- Pillow

## Usage

1. **Mount Google Drive:**
   - Mount your Google Drive to access the dataset stored there. The dataset is not a complicated and it got few datasets. The dataset is already included on this repossitory with a folder plant_doctor

2. **Set the path to your dataset within Google Drive:**
   - Update the `data_dir` variable with the path to the plant_doctor dataset on your Google Drive.

3. **Define Image Transformations for Preprocessing:**
   - The `transform` variable contains the required transformations for image preprocessing.

4. **Create a Dataset and Split into Training and Testing Sets:**
   - The dataset is created using the ImageFolder class, assuming each subfolder in `data_dir` represents a different class.
   - The dataset is split into training and testing sets.

5. **Create a DataLoader for Efficient Data Loading:**
   - Utilize DataLoader to efficiently load and batch the data.

6. **Define and Train the Baseline CNN Model:**
   - A baseline CNN model (`BaselineModel`) is defined and trained using a specified criterion and optimizer.

7. **Evaluate the Model on the Test Dataset:**
   - The model's performance is evaluated on the test dataset, and the test accuracy is printed.

8. **Save the Trained Model:**
   - The trained model is saved as 'baseline_model.pth' for reuse in predictions or further training.

9. **Load the Model for Further Use:**
   - The model architecture is loaded, and its weights are loaded from the saved file.

10. **Make Predictions on a New Image:**
    - A new image is preprocessed, passed through the loaded model, and its predicted class label and confidence are printed.

## Note
- Ensure that your dataset is structured in subfolders, each representing a different class.
- The provided model architecture (`BaselineModel`) is a simple example and may need adjustments based on the complexity of the dataset.

Feel free to customize the project based on your specific dataset and requirements.
