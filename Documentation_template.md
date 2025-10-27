# ML Challenge 2025: Smart Product Pricing Solution.

**Team Name:**  - Team
**Team Members:**  - Shalini Karta
                   - Ommprakash Jena
                   - Prachi Parimita Chulli 
**Submission Date:** [13/10/25]

## 1. Executive Summary
We built a smart product pricing system that predicts prices using both text descriptions and product images. Our solution uses machine learning to analyze text content and color features from images to estimate product prices automatically.

## 2. Methodology Overview

### 2.1 Problem Analysis
We looked at the product pricing challenge and found that prices depend on many factors like product descriptions, visual features, and market positioning. The main challenge was extracting useful information from both text and images to make accurate price predictions.

**Key Observations:**

1. Product descriptions contain valuable keywords that hint at pricing (luxury, premium, cheap, affordable).

2. Images provide visual cues through color patterns and features.

3. Price prediction is complex because many external factors affect pricing.

4. Combining text and image data gives better results than using just one type.

### 2.2 Solution Strategy
We used a multimodal approach that combines both text and image processing to predict product prices.

**Approach Type:**  Multimodal Machine Learning  
**Core Innovation:**  Combined text analysis using TF-IDF with image color feature extraction and Ridge regression for final price prediction.


## 3. Model Architecture

### 3.1 Architecture Overview
 Our system works in three main steps:

1. Text Processing: Extract features from product descriptions using TF-IDF and keyword counting

2. Image Processing: Extract color histograms and visual features from product images

3. Price Prediction: Combine all features and use Ridge regression to predict the final price


### 3.2 Model Components

**Text Processing Pipeline:**
- [ ] Preprocessing steps: Text cleaning, removing special characters, converting to lowercase

- [ ] Model type: TF-IDF Vectorizer with Ridge Regression

- [ ] Key parameters: max_features=3000, ngram_range=(1,2), stop_words='english'


**Image Processing Pipeline:**
- [ ] Preprocessing steps: Image resizing, color space conversion

- [ ] Model type: Color histogram extraction

- [ ] Key parameters: RGB color histograms, histogram binning


## 4. Model Performance

### 4.1 Validation Results
Our model achieved the following performance metrics:

**SMAPE Score**: 71.48%

**Mean Absolute Error (MAE)**: 16.13

**Root Mean Squared Error (RMSE)**: 35.98

**R-Squared (Accuracy Rate)**: 14.21% 

### Performance analysis

**The model accuracy of 14.21% reflects the complexity of real-world product price prediction. Here's why this is actually reasonable:**

## Reasons for current accuracy level:   ( ##important)

Product pricing depends on many external factors like brand value, market demand, and seasonal trends that are not available in the dataset.

The model only uses basic text and image features, while real pricing involves complex business decisions.

Time constraints limited advanced feature engineering and model optimization.

Despite the modest accuracy, our model provides a solid foundation that can be improved with more data and features.

## What this means:

Our model can capture some pricing patterns and provides useful predictions

The system is built to be easily improved by adding more features or better algorithms

For a baseline model, this performance shows the approach is working and can be enhance


## 5. Conclusion
We successfully created a multimodal machine learning system that predicts product prices by analyzing both text descriptions and image features. While our current accuracy is 14.21%, this represents a solid foundation for automated pricing that can be improved with more sophisticated features and larger datasets. The project demonstrates practical application of machine learning to real business problems.

## Appendix

### A. Code artefacts
Complete Jupyter notebook with all preprocessing, feature extraction, model training, and evaluation code.

### B. Additional Results
All charts, visualizations, and detailed performance metrics are included in the notebook.

**Technical Implementation Details:**

- Used Python with scikit-learn, pandas, and numpy

- Processed both text and image data simultaneously

- Applied Ridge regression for stable predictions

- Included comprehensive error analysis and validation metrics

### This solution provides a practical approach to automated product pricing that businesses can build upon and improve over time.


