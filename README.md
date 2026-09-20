#AICTE Internship Projects

This repository contains three machine learning and computer vision projects completed as part of my AICTE internship. Each project focuses on a different practical application of AI/ML, covering unsupervised learning, natural language processing, and object detection.

Projects in this Repository

Customer Segmentation using K-Means Clustering

Sentiment Analysis on Movie Reviews

YOLOv8-Based Object Detection

1. Customer Segmentation using K-Means Clustering

1. Problem Statement

Businesses often have customers with different spending patterns and purchasing behaviours. Treating all customers in the same way makes it difficult to understand which groups of customers are high-value, moderate-value, or less engaged.

The problem is to identify meaningful customer groups from customer-related numerical data without having predefined customer categories.

2. Proposed Solution

A K-Means Clustering model is used to divide customers into groups with similar characteristics.

For this project, the Mall Customers dataset is used. Customer attributes are analysed and customers are grouped based on their similarities. The resulting clusters can help in understanding different customer segments and can support targeted marketing and customer-management strategies.

The model uses K = 5 clusters for segmentation.

3. Methodology / Workflow

Mall Customers Dataset
        ↓
Data Loading
        ↓
Data Exploration
        ↓
Feature Selection
        ↓
Data Preprocessing
        ↓
K-Means Clustering
        ↓
Customer Groups / Clusters
        ↓
Cluster Visualization
        ↓
Cluster Evaluation

The clustering process includes:

Loading and exploring the customer dataset.

Selecting suitable features for segmentation.

Applying K-Means clustering.

Dividing customers into five clusters.

Visualizing the resulting customer groups.

Evaluating the quality of clustering using clustering metrics.

4. Technologies Used

Python

Pandas

NumPy

Matplotlib

Scikit-learn

K-Means Clustering

Mall Customers dataset

Jupyter Notebook / Google Colab

5. Implementation

The implementation follows these main steps:

Load the Mall Customers dataset.

Inspect the dataset and understand the available customer attributes.

Select the features required for clustering.

Prepare the data for the K-Means algorithm.

Set the number of clusters to 5.

Train the K-Means model.

Assign each customer to a cluster.

Visualize the customer clusters.

Calculate clustering evaluation metrics.

The implementation is focused on unsupervised learning, where the model discovers groups from the data instead of using predefined class labels.

6. Results / Outputs

The model produces:

Five customer clusters.

Cluster assignments for individual customers.

Visual representations of the customer segments.

Cluster-quality evaluation metrics.

The recorded evaluation values for this project include:

Silhouette Score: approximately 0.598

Calinski-Harabasz Score: approximately 3306.810

These metrics were used to assess how well the customers were separated into clusters.

7. Learning Outcomes

Through this project, I learned:

The concept of unsupervised learning.

How K-Means clustering works.

How to select data features for clustering.

How clustering differs from classification.

How to interpret customer segments.

How to visualize clusters.

How to evaluate clustering using Silhouette Score and Calinski-Harabasz Score.

8. Future Improvements

Possible improvements include:

Testing different values of K and comparing clustering quality.

Applying feature scaling and studying its effect on the clusters.

Adding more customer attributes.

Comparing K-Means with other clustering algorithms such as DBSCAN or hierarchical clustering.

Building a dashboard to interactively explore customer segments.

Connecting the segmentation output to a recommendation or marketing system.

9. Project Status

Status: Completed as an AICTE internship project

The project demonstrates a practical implementation of K-Means clustering for customer segmentation using the Mall Customers dataset.

2. Sentiment Analysis on Movie Reviews

1. Problem Statement

Movie reviews contain opinions that can be useful for understanding whether viewers had a positive or negative experience. Manually analysing a large number of reviews is time-consuming.

The problem is to automatically classify movie reviews according to their sentiment.

2. Proposed Solution

A text-classification pipeline is developed using TF-IDF for converting review text into numerical features and Logistic Regression for classifying the reviews.

The project focuses on positive and negative sentiment classification using movie-review data.

3. Methodology / Workflow

Movie Review Dataset
        ↓
Text Data Preparation
        ↓
Text Preprocessing
        ↓
TF-IDF Feature Extraction
        ↓
Logistic Regression
        ↓
Sentiment Prediction
        ↓
Model Evaluation
        ↓
Confusion Matrix / ROC Curve

The workflow includes:

Loading movie-review data.

Preparing the text data.

Converting text into numerical TF-IDF features.

Training a Logistic Regression classifier.

Predicting sentiment labels.

Evaluating the classification results.

4. Technologies Used

Python

Pandas

NumPy

Scikit-learn

TF-IDF

Logistic Regression

Matplotlib

Natural Language Processing (NLP)

Movie Reviews dataset

Jupyter Notebook / Google Colab

5. Implementation

The implementation follows these steps:

Load the movie-review dataset.

Prepare the review text and sentiment labels.

Perform the required text preprocessing.

Convert the review text into TF-IDF vectors.

Split the data into training and testing data.

Train a Logistic Regression model.

Predict the sentiment of test reviews.

Evaluate the predictions using classification metrics.

Generate a confusion matrix and ROC curve for additional evaluation.

The project demonstrates a traditional and interpretable NLP classification pipeline rather than using a large language model.

6. Results / Outputs

The project produces:

Predicted sentiment labels for movie reviews.

Model evaluation results.

A confusion matrix showing correct and incorrect classifications.

An ROC curve and ROC-AUC evaluation for the classifier.

The model classifies reviews into:

Positive

Negative

7. Learning Outcomes

Through this project, I learned:

Basic concepts of Natural Language Processing.

How text data can be converted into numerical features.

TF-IDF feature extraction.

Text classification using Logistic Regression.

Training and testing an NLP model.

Interpreting a confusion matrix.

Understanding ROC curves and ROC-AUC.

The importance of evaluating a classification model using multiple metrics.

8. Future Improvements

Possible improvements include:

Adding a neutral sentiment class.

Improving text preprocessing.

Comparing Logistic Regression with models such as Naive Bayes, SVM, or neural networks.

Using word embeddings or transformer-based models.

Handling sarcasm, negation, and context-dependent sentiment.

Developing a simple web application for real-time review classification.

9. Project Status

Status: Completed as an AICTE internship project

The project demonstrates an end-to-end NLP classification workflow for identifying positive and negative sentiment in movie reviews.

3. YOLOv8-Based Object Detection

1. Problem Statement

Object detection systems are required in many real-world applications such as surveillance, industrial inspection, traffic monitoring, and automated visual analysis.

The problem is to detect and locate objects in images using a custom dataset instead of relying only on predefined datasets and classes.

2. Proposed Solution

A custom object-detection solution is developed using YOLOv8n. The dataset is prepared using Roboflow and then used to train and evaluate the YOLOv8 object-detection model.

The system identifies the trained object classes in an image and produces bounding boxes around detected objects.

3. Methodology / Workflow

Custom Image Dataset
        ↓
Dataset Preparation / Annotation
        ↓
Roboflow Dataset Management
        ↓
Train / Validation / Test Split
        ↓
YOLOv8n Model
        ↓
Model Training
        ↓
Model Validation
        ↓
Object Detection on Images
        ↓
Bounding Boxes + Class Predictions
        ↓
Precision / Recall / mAP Evaluation

The workflow includes:

Collecting and preparing the custom image dataset.

Annotating the required object classes.

Preparing the dataset using Roboflow.

Training the YOLOv8n model.

Validating the trained model.

Running object detection on images.

Visualizing the detections.

Evaluating the model using detection metrics.

4. Technologies Used

Python

YOLOv8n

Ultralytics

Roboflow

OpenCV

NumPy

Matplotlib

Computer Vision

Object Detection

Jupyter Notebook / Google Colab

5. Implementation

The implementation follows these steps:

Prepare the custom image dataset.

Annotate the objects required for detection.

Organize the dataset into training, validation, and test data.

Use Roboflow for dataset preparation and export.

Load the YOLOv8n model using the Ultralytics framework.

Train the model using the custom dataset.

Validate the model.

Run inference on images.

Display bounding boxes and class labels on detected objects.

Evaluate the model using Precision, Recall, and mAP.

The implementation uses OpenCV for image-related operations and Matplotlib for visualization.

6. Results / Outputs

The project produces:

Object detections from input images.

Bounding boxes around detected objects.

Predicted class labels.

Visualized detection results.

Model evaluation results using:

Precision

Recall

mAP

The project demonstrates how a pretrained YOLOv8 architecture can be adapted for custom object-detection tasks.

7. Learning Outcomes

Through this project, I learned:

Fundamentals of computer vision.

The difference between image classification and object detection.

How object-detection datasets are annotated.

Custom dataset preparation using Roboflow.

Basic YOLOv8 workflow.

Training and validating an object-detection model.

Running inference on images.

Understanding Precision, Recall, and mAP in object detection.

Visualizing bounding-box predictions.

8. Future Improvements

Possible improvements include:

Increasing the size and diversity of the training dataset.

Improving annotation quality.

Testing larger YOLOv8 model variants.

Applying data augmentation.

Tuning training parameters.

Evaluating the model under different lighting and environmental conditions.

Deploying the detector through a web or mobile application.

Optimizing the model for real-time edge-device inference.

9. Project Status

Status: Completed as an AICTE internship project

The project demonstrates a custom YOLOv8-based object-detection workflow, from dataset preparation and training to inference and evaluation.

Skills Developed Across the Internship Projects

Working on these three projects provided practical exposure to multiple areas of AI and machine learning:

Python programming

Data preprocessing

Data analysis and visualization

Unsupervised learning

K-Means clustering

Natural Language Processing

TF-IDF

Logistic Regression

Computer Vision

Object Detection

YOLOv8

Roboflow

Model training and evaluation

Performance metrics

Jupyter Notebook / Google Colab

Overall Learning Outcome

The three projects provided experience across different AI/ML problem types:

Project

Domain

Main Technique

Customer Segmentation

Machine Learning

K-Means Clustering

Sentiment Analysis

NLP

TF-IDF + Logistic Regression

Object Detection

Computer Vision

YOLOv8n

This repository therefore represents an internship portfolio covering unsupervised machine learning, NLP-based classification, and computer vision-based object detection.

Repository Structure

AICTE-internship-projects/
│
├── Mall_Customer_Segmentation_.../
├── Sentiment_Analysis_on_movie_reviews_.../
├── yolov8_Based_on_Object_Detection_.../
└── README.md

Author

Hima Harshitha Janjanam
B.Tech – Computer Science and Engineering (AI & ML)

This repository contains projects completed as part of my AICTE internship and is maintained as part of my academic and professional portfolio.
