
### COMP3314_assignment3

- Project Overview
  - This project is designed for image classification tasks, utilizing multiple feature extraction techniques such as HOG, LBP, and SIFT combined with PCA for dimensionality reduction and SVM for classification. The aim of this project is to demonstrate how different feature extraction methods and model training techniques can be applied to handle image classification problems.

## Dataset

- Kaggle dataset
  - url: `kaggle competitions download -c 2025-hku-comp-3314-image-classification-challenge`
  - download the dataset from kaggle and put the `image_classification.py` and fold `data` under the same fold
 
## Install Dependencies

- The project relies on the following libraries:
    - `pandas`
    - `numpy`
    - `matplotlib`
    - `scikit-learn`
    - `opencv-python`
    - `scikit-image`
    - `tqdm`
    - `lightgbm`
    - `seaborn`
    - `cuml` (for GPU-accelerated machine learning)


## Features

- Data Loading and Preprocessing
    - Load image paths and labels from CSV files
    - Read images using OpenCV
    - Enhance contrast (using CLAHE)
    - Apply bilateral filtering
- Feature Extraction
    - Histogram of Oriented Gradients (HOG): Extracts edge and texture features
    - Local Binary Patterns (LBP): Extracts local texture features
    - HSV Color Space: Extracts features based on HSV color space
    - Scale-Invariant Feature Transform (SIFT): Extracts keypoint descriptors
    - FAST: Fast feature point detection
    - DAISY: Image descriptor calculation
- Feature Combination and Transformation
    - Apply PCA (Principal Component Analysis) to reduce the dimensionality of each feature
    - Combine all features into a comprehensive feature vector
- Model Training and Testing
    - Train and test using Support Vector Machine (SVM) classifier
    - Train and test using Logistic Regression model
    - Print classification results and confusion matrix
## Project Results
- Accuracy
    - Accuracy of the SVM classifier: 71.17%
    - Accuracy of the LGB classifier: 61.98%
- Confusion Matrix
    - The confusion matrix helps us understand the classification performance for each category.
    - ![image](https://github.com/user-attachments/assets/a6a230a2-ec05-4658-aa33-a2aafeb41002)

    - ![image](https://github.com/user-attachments/assets/2f29b72a-e2a5-423d-b899-762109f5c005)

 
## Authors

- [@Zhang_Shenru](https://www.github.com/mkyahx)

- [@Chen_Liangyi](https://www.github.com/eddieidde04)

- [@Li_Hewen](https://www.github.com/JackLihh)
## License

[MIT](https://choosealicense.com/licenses/mit/)




    
