# Sentiment Analysis Using Gemini LLM and Chain-of-Thought Prompting

## 📌 Project Overview

This project demonstrates how Large Language Models (LLMs) can be used for sentiment analysis without traditional machine learning training.

The workflow involves collecting customer reviews from Amazon, cleaning the text data, and leveraging Google's Gemini model to classify reviews into:

* Positive
* Negative
* Neutral

The project also explores the impact of **Chain-of-Thought (CoT) Prompting**, where the model is encouraged to reason step-by-step before producing the final sentiment label.

---

##  Problem Statement

Customer reviews contain valuable insights about products and services. However, manually analyzing thousands of reviews is time-consuming and inefficient.

The objective of this project is:

> To automatically classify customer reviews into sentiment categories using a Large Language Model (Gemini) and evaluate how prompt engineering techniques influence model performance.

---

##  Project Objectives

* Extract customer reviews from Amazon product pages
* Clean and preprocess raw review text
* Perform sentiment classification using Gemini LLM
* Compare standard prompting with Chain-of-Thought prompting
* Understand how reasoning-based prompts affect sentiment prediction

---

##  Project Workflow

### Step 1: Data Collection

Customer reviews are collected from Amazon product pages using:

* Requests
* BeautifulSoup

### Step 2: Text Preprocessing

Review text is cleaned by:

* Removing unwanted characters
* Handling encoding issues
* Eliminating extra spaces
* Formatting sentences

### Step 3: Prompt Engineering

Two prompt designs are evaluated:

#### Version 1

Basic sentiment classification prompt.

#### Version 2

Enhanced prompt with:

* Explicit sentiment instructions
* Better role definition
* Structured classification requirements

### Step 4: Chain-of-Thought Reasoning

The Gemini model is encouraged to:

* Analyze sentiment-bearing phrases
* Identify positive and negative indicators
* Reason through the review
* Generate a final sentiment classification

### Step 5: Sentiment Prediction

The model returns one of:

* Positive
* Negative
* Neutral

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* BeautifulSoup
* Requests
* Regex

### Generative AI

* Google Gemini
* LangChain Google Generative AI

### Development Environment

* Google Colab
* Jupyter Notebook

---

## 📂 Project Structure

```text
Sentiment-with-CoT.ipynb
│
├── Amazon Review Scraping
├── Data Cleaning
├── Prompt Engineering
├── Gemini API Integration
├── Chain-of-Thought Prompting
└── Sentiment Classification
```

---

##  Chain-of-Thought Prompting

Chain-of-Thought (CoT) prompting encourages the model to break down its reasoning process before arriving at a final prediction.

Example:

```text
Review
↓
Analyze key phrases
↓
Identify sentiment indicators
↓
Reason step-by-step
↓
Final Sentiment Label
```

Benefits:

* Improved reasoning
* Better transparency
* More reliable sentiment classification

---

##  Example Output

### Input Review

> "The battery life is excellent and easily lasts two days. The display is smooth and immersive."

### Model Prediction

```text
Positive
```

---

##  Key Learnings

* Prompt design significantly impacts LLM performance.
* Chain-of-Thought prompting improves reasoning quality.
* LLMs can perform sentiment analysis without traditional model training.
* Prompt engineering is a powerful technique in Generative AI applications.

---

##  Future Enhancements

* Batch sentiment analysis
* Aspect-based sentiment analysis
* Sentiment score generation
* Multi-language review classification
* Streamlit deployment
* Comparison with traditional ML models

---

##  Potential Applications

* Product Review Analysis
* Brand Monitoring
* Customer Feedback Analytics
* E-commerce Insights
* Social Media Sentiment Tracking

---

##  Author

**Hadwala Akhil**

Data Science | Machine Learning | Generative AI Enthusiast

---

##  Key Takeaway

> Traditional Machine Learning learns sentiment from training data.
> Large Language Models can infer sentiment directly through prompting and reasoning, making sentiment analysis faster, more flexible, and easier to deploy.
