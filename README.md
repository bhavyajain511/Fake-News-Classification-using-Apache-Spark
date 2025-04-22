# 📰 Fake News Detection with Apache Spark

This project aims to detect fake news using Natural Language Processing (NLP) and Apache Spark's scalable machine learning libraries. It includes exploratory data analysis, preprocessing steps, model training, and a presentation of results.

## 📁 Project Structure

- `EDA.ipynb` – Exploratory Data Analysis to understand the dataset, identify key features, and detect missing values.
- `Final Project.ipynb` – Full implementation of the fake news classification model using Apache Spark.
- `Presentation.pptx` – Slide deck summarizing the project, problem statement, methodology, and results.
- `Presentation-pdf.pdf` – PDF version of the project presentation for quick viewing.
- `model and pipeline/` – Contains the serialized Naive Bayes model and the Spark MLlib pipeline used for training and inference.

## 📌 Problem Statement

Fake news undermines public trust, spreads misinformation, and can cause real-world consequences such as:
- Social unrest
- Economic damage
- Public health risks

## 📊 Dataset Overview

- **Source**: Kaggle (contributed by William Lifferth)
- **Size**: ~20,000 articles (~100MB)
- **Key Features**: `title`, `author`, `text`, `label (real/fake)`

## 🔍 Exploratory Data Analysis (EDA)

- **Feature Identification**: Irrelevant features like `author` were dropped.
- **Missing Value Analysis**: News missing key features were likely to be fake.

## ⚙️ Preprocessing Steps

1. Text cleaning (lowercasing, removing non-alphanumeric characters)
2. Stopword removal using NLTK
3. Stemming with PorterStemmer
4. Vectorization using TF-IDF

## 🤖 Model Details

- **Algorithm**: Naive Bayes (efficient for text classification)
- **Library**: Apache Spark MLlib
- **Tuning**: Grid search and cross-validation for best parameters
- **Model & Pipeline Storage**:
  - The trained Naive Bayes model and preprocessing pipeline are saved in the `model and pipeline/` folder for reproducibility and future inference.

## ⚡ Apache Spark Advantage

- Distributed and parallel processing with **Spark Core**
- Scalable ML algorithms with **Spark MLlib**
- Structured data handling via **Spark SQL**

## 📈 Results

| Metric     | Value   |
|------------|---------|
| Accuracy   | 92.5%   |
| Precision  | 97.2%   |
| F1-Score   | 93.0%   |

## 🌍 Impact

- Enhances public awareness by identifying misinformation
- Builds trust in media platforms
- Promotes a safer digital environment

## 👨‍💻 Contributors

- **Bhavya Jain** 
- **Divyansh Saharan**
- **Kushagra Agarwal**
