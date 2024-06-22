# Mini-Project for Fundamentals of Machine Learning Course
![background](./materials/ai_wp.jpg)
This repository contains the code and data for a mini-project on facial expression recognition using machine learning algorithms.

## 📑 Project Policy
- Team: group should consist of 3-4 students.

    |No.| Student Name    | Student ID |
    | --------| -------- | ------- |
    |1| Võ Thị Khánh Linh | 21280070 |
    |2| Lê Quang Trung | 21280113 |
    |3| Nguyễn Nhật Minh Thư | 21280112|
    |4| Nguyễn Đặng Anh Thư | 21280111 |

- The submission deadline is strict: **11:59 PM** on **June 22nd, 2024**. Commits pushed after this deadline will not be considered.

## 📦 Project Structure

The repository is organized into the following directories:

- **/data**: This directory contains the facial expression dataset. You'll need to download the dataset and place it here before running the notebooks. (Download link provided below)
- **/notebooks**: This directory contains the Jupyter notebook ```EDA.ipynb```. This notebook guides you through exploratory data analysis (EDA) and classification tasks.

## ⚙️ Usage

This project is designed to be completed in the following steps:

1. **Fork the Project**: Click on the ```Fork``` button on the top right corner of this repository, this will create a copy of the repository in your own GitHub account. Complete the table at the top by entering your team member names.

2. **Download the Dataset**: Download the facial expression dataset from the following [link](https://mega.nz/file/foM2wDaa#GPGyspdUB2WV-fATL-ZvYj3i4FqgbVKyct413gxg3rE) and place it in the **/data** directory:

3. **Complete the Tasks**: Open the ```notebooks/EDA.ipynb``` notebook in your Jupyter Notebook environment. The notebook is designed to guide you through various tasks, including:
    
    1. Prerequisite
    2. Principle Component Analysis
    3. Image Classification
    4. Evaluating Classification Performance 

    Make sure to run all the code cells in the ```EDA.ipynb``` notebook and ensure they produce output before committing and pushing your changes.

5. **Commit and Push Your Changes**: Once you've completed the tasks outlined in the notebook, commit your changes to your local repository and push them to your forked repository on GitHub.


Feel free to modify and extend the notebook to explore further aspects of the data and experiment with different algorithms. Good luck.

## 📑 Improvemnts: 

Apart from the given questions, our group has made the following improvements:

1. Feature Engineering: We utilized the Histogram of Oriented Gradients (HOG) algorithm to extract features from images. HOG is effective in representing the main contours of the face by capturing the direction and magnitude of gradients through vectors in each cell.
2. Handling Classification with Imbalanced Datasets: One effective technique for addressing class imbalance is the strategic use of class weights. Class weights assign higher weights to the minority class, allowing the model to pay more attention to its patterns and reducing bias towards the majority class.

## 📦 Observations about different models and feature engineering techniques:

Model Performance on Different Data Representations:
1. Original Data and PCA Transformed Data: Random Forest emerged as the best performing model for both the original dataset and the PCA-transformed dataset. Its ensemble nature, which aggregates the predictions of multiple decision trees, contributed to its robust performance by effectively capturing the underlying patterns in these datasets.
2. HOG Features: Support Vector Classifier (SVC) outperformed other models when HOG features were used. The SVC's ability to handle high-dimensional data and complex decision boundaries through kernel functions allowed it to leverage the detailed and informative features extracted by the HOG algorithm, leading to superior classification results.

These observations underscore the importance of choosing the right model based on the specific characteristics of the feature representation. While Random Forest excelled with the original and PCA-transformed data, the SVC demonstrated its strength with the more sophisticated HOG features.
## 📑 Futureworks: 

1. Transfer Learning: use VGG16, VGG19, or MobileNet as the base model for our classification tasks. These pre-trained models provide a strong foundation by leveraging their ability to extract robust features from images, enhancing the overall performance of our classifier.
2. CNN: train a full Convolutional Neural Network (CNN) for classification, as CNNs have the capability to automatically extract features from images, making them well-suited for tasks of this nature.
3. Data Augmentation: Data augmentation involves creating new training samples by applying various transformations to existing images, thereby increasing the diversity of the dataset and mitigating the effects of class imbalance.
