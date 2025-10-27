Smart Product Pricing Prediction
This repository contains a machine learning solution for the Smart Product Pricing Challenge 2025. The project aims to predict prices for e-commerce products by leveraging both text descriptions and product images using multimodal machine learning techniques.

Project Overview
The problem involves estimating product prices based on various features extracted from textual product description data and visual features from product images. This project implements a multimodal approach combining TF-IDF vectorization for text data and color histogram-based features for images.

Solution Approach
Data Processing: Textual features were extracted using TF-IDF on product descriptions, along with handcrafted features such as keyword counts. Image features were extracted using color histograms capturing RGB channels.

Model: A Ridge regression model was trained using combined text and image features creating a robust baseline for price prediction.

Performance: The model achieved a SMAPE of approximately 71.48% and an R-squared accuracy of 14.21%, reflecting real-world pricing complexity.

Pipeline: The solution includes data preprocessing, feature extraction, model training, and validation stages, packaged in easy-to-follow notebooks.

Contents
Smartproductpricing.ipynb: The Jupyter notebook containing the full code implementation including data loading, preprocessing, modeling, and evaluation.

Documentation_template.md: Detailed project documentation explaining methodology, architecture, results, and conclusions.

Additional CSV files used for training and testing.

Usage
Clone the repository and run the notebook in a compatible environment with required dependencies (scikit-learn, pandas, numpy, opencv-python, etc.). Follow the notebook to understand data processing steps and generate price predictions on test data.

Future Work
The current solution establishes a foundation for automated product price prediction but leaves room for improvement through deeper feature engineering, advanced modeling techniques, and hyperparameter tuning.

