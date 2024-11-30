# Sentiment Analysis Using Natural Language Processing (NLP)

## Overview
This project demonstrates the process of sentiment analysis, a widely-used application in Natural Language Processing (NLP). The goal is to classify text into **positive**, **negative**, or **neutral** sentiments using machine learning techniques.

### Applications
- **E-commerce**: Analyze customer reviews to improve product quality.
- **Social Media Monitoring**: Understand public sentiment toward brands or events.
- **Customer Support**: Detect dissatisfaction to enhance service.

---

## Steps in the Pipeline

### **1. Loading and Exploring the Dataset**
- **Dataset**: The [NLTK Movie Reviews Dataset](https://www.nltk.org/nltk_data/) contains movie reviews labeled as **positive** or **negative**.
- **Objective**: Understand the structure of the dataset and identify any cleaning requirements.

### **2. Text Preprocessing**
- Convert text to lowercase for consistency.
- Remove punctuation and stop words (common words like "the" and "is").
- Tokenize sentences into words.
- Perform stemming to reduce words to their root forms (e.g., "running" → "run").

### **3. Feature Extraction Using TF-IDF**
- **TF-IDF (Term Frequency-Inverse Document Frequency)** is used to transform text into numerical features, emphasizing significant words while reducing the weight of commonly occurring terms.

### **4. Model Training**
- Train a **Naive Bayes Classifier** on the TF-IDF features.
- Split the dataset into training and testing sets to evaluate performance.

### **5. Model Evaluation**
- Metrics:
  - **Accuracy**: Measures overall model performance.
  - **Precision, Recall, and F1-Score**: Detailed evaluation for each class.
- Visualize errors using a confusion matrix.

### **6. Word Cloud Visualization**
- Generate word clouds for positive and negative reviews to highlight frequently used words for each sentiment.

---

## Results and Insights

### **Key Insights**
1. **Text Preprocessing**: Improved data quality and ensured meaningful feature extraction.
2. **Model Performance**: The Naive Bayes classifier achieved high accuracy, effectively distinguishing positive and negative sentiments.
3. **Visualization**: Word clouds highlighted key terms associated with each sentiment.

### **Applications**
- Monitor customer reviews to improve products.
- Analyze social media sentiment to manage brand reputation.
- Detect dissatisfaction in customer support.

### **Next Steps**
- Experiment with advanced models like Logistic Regression, Random Forest, or BERT.
- Use larger, more diverse datasets for improved generalization.
- Extend the project to real-world applications like spam detection or emotion classification.

---

## How to Run

1. Clone the repository and install dependencies:
   ```bash
   pip install -r requirements.txt
