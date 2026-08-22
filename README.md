# CNN-Based Fruit Freshness Classification Model to Support Automated Sorting and Quality Control with ResNet50 Transfer Learning

An image classification project developed as part of the Komputasi Statistika II practicum at Universitas Gadjah Mada (UGM) to classify the freshness condition of fruits and potatoes based on images.
The model classifies images into 8 categories consisting of fresh and rotten apples, oranges, potatoes, and tomatoes.

Manual inspection of fruit freshness can be subjective and time-consuming. This project explores the use of Computer Vision and Deep Learning to automate the classification process based on visual characteristics.
A pretrained ResNet50 architecture was implemented using transfer learning. The pretrained model was adapted to classify images into eight freshness categories.

The project covers:
- Exploratory Data Analysis
- Image preprocessing
- Data augmentation
- Class imbalance handling
- Transfer learning
- Model training
- Model evaluation
- Image classification

## Libraries Used
- TensorFlow / Keras — for building, training, and evaluating the CNN model.
- NumPy — for numerical computations and array manipulation.
- Pandas — for data processing and analysis.
- Matplotlib — for data visualization and plotting training results.
- Seaborn — for statistical visualization and confusion matrix visualization.
- Scikit-learn — for model evaluation, including classification reports and confusion matrices.
- Pillow (PIL) — for image processing and manipulation.

## Dataset
The dataset used in this study consists of digital images of four major food commodities: apples, tomatoes, oranges, and potatoes. Each commodity is categorized into two freshness levels, namely fresh and rotten, resulting in a total of eight classes. The dataset is designed to support image classification using computer vision techniques to distinguish between fresh and rotten food products.

For model training and evaluation, the dataset is divided into three main subsets: the training set, validation set, and test set. The training set consists of 13,754 images, which are used to train the model to recognize visual patterns that distinguish between fresh and rotten products. The validation set contains 2,676 images and is used to evaluate model performance periodically during the training process, as well as to help detect potential overfitting or underfitting. Meanwhile, the test set consists of 724 unlabeled images and is used to objectively measure the final performance of the classification model through an automated evaluation system. 
The training dataset contains an imbalance between classes. Therefore, WeightedRandomSampler was used during training to provide a more balanced contribution from each class.

