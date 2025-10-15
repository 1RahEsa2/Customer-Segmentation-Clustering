Know Your Customers, Grow Your Business: A Segmentation Analysis

# Customer Segmentation & Buying Behavior Analysis
Know Your Customers, Grow Your Business: A Segmentation Analysis

## 📊 Project Overview

A comprehensive data science project that analyzes customer purchasing behavior and segments customers into meaningful groups using unsupervised machine learning techniques. This project transforms raw transaction data into actionable business insights through rigorous statistical analysis, feature engineering, and advanced clustering algorithms.

## 🎯 Project Objectives

- **Customer Behavior Analysis**: Deep dive into purchasing patterns, regional preferences, and transaction characteristics
- **Data Quality Assessment**: Identify and address data quality issues including outliers and statistical anomalies
- **Customer Segmentation**: Group customers into distinct clusters based on purchasing behavior
- **Strategic Insights**: Provide data-driven recommendations for marketing, inventory, and customer service

## 📁 Dataset & Features

### Original Features:
- **Cust ID** - Unique customer identifier
- **Region** - Geographic location (East, West, North, South)
- **Payment_mode** - Payment method (Credit, Paypal)
- **how_they_buy** - Purchase channel (Web, Email)
- **Amount_in_usd** - Transaction value
- **Product_type** - Category of product (Online, Book)
- **Time Of Day** - Transaction timestamp

## 🔧 Data Processing Pipeline

### 1. Data Quality & Statistical Assessment
- Comprehensive statistical analysis of numerical and categorical variables
- Outlier detection and treatment strategies
- Null value analysis across all features
- Skewness evaluation for numerical columns

### 2. Feature Engineering
**Temporal Features:**
- `Hour_of_Day` - Extracted hour component from timestamp
- `Time` - Converted to total minutes for numerical analysis
- `hour_groups` - Categorized into meaningful time segments:
  - 12am to 6am, 6am to 12pm, 12pm to 6pm, 6pm to 12am
- `Hour_Group_Num` - Numerical encoding of time segments

**Business Logic Features:**
- `Sales_Less_Than_50` - Binary indicator for small vs large purchases
- Enhanced categorical representations for better analysis

### 3. Exploratory Data Analysis
**Multi-dimensional Analysis:**
- Relationships between numerical features (Amount_in_usd vs Time)
- Categorical feature distributions (Region, Payment_mode, Product_type)
- Cross-analysis between numerical and categorical variables
- Temporal patterns and regional purchasing behaviors

## 🛠️ Advanced Analytical Methodology

### Feature Selection Strategy
**Supervised Approach for Unsupervised Problem:**
- Converted to supervised learning using `Product_type` as target variable
- Assessed feature importance for product type discrimination
- Selected most impactful features for clustering
- Applied PCA on selected features for dimensionality reduction

### Preprocessing Pipeline
1. **Column Removal**: Eliminated unnecessary features
2. **Value Normalization**: Unified value ranges across features
3. **Categorical Encoding**: Converted categorical variables to numerical representations
4. **Feature Scaling**: Applied normalization for clustering algorithms

## 🤖 Machine Learning Modeling

### Clustering Algorithms Implemented:
- **DBSCAN** - Density-based spatial clustering
- **K-Means** - Centroid-based partitioning
- **Agglomerative Clustering** - Hierarchical clustering approach

### Cluster Quality Assessment:
- **Silhouette Score** - Measuring cluster cohesion and separation
- **Dendrogram Analysis** - Visual hierarchy for cluster determination
- **Elbow Method** - Optimal cluster number selection
- **Multiple Validation Techniques** - Comprehensive cluster evaluation

## 📈 Results & Business Insights

### Cluster Analysis:
- **Waffle Chart Visualization**: Percentage distribution of each cluster
- **Cluster Statistics**: Mean values and characteristics per segment
- **Behavioral Profiles**: Detailed understanding of each customer group


