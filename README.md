Fake News Detection using Machine Learning

This project explores how machine learning can be used to identify fake news articles.  
Using TF-IDF for text vectorization and two different classifiers — **Logistic Regression** and **Decision Tree** — the model predicts whether a given news article is real or fake.

The goal of the project was to build a simple, easy-to-understand end-to-end pipeline for text classification.

---

 Overview

Fake news has become a major challenge in the digital world.  
In this project, I used a Kaggle dataset containing both **real** and **fake** news articles. After cleaning and processing the text, I trained two models and compared their performance.

The project includes:

- Data loading and exploration  
- Text cleaning and preprocessing  
- TF-IDF vectorization  
- Model training (LR & Decision Tree)  
- Accuracy comparison  
- A manual testing function to test custom news text  



 Dataset

The dataset consists of two files:

- `true.csv` — Real news articles  
- `fake.csv` — Fake news articles  

Both datasets include the article text and metadata.  
Only the **text** column was used for training the models.

You can download the dataset here:  
(https://www.kaggle.com/datasets/bhavikjikadara/fake-news-detection)



Text Preprocessing

I created a simple preprocessing function `wordopt()` that:

- Converts text to lowercase  
- Removes URLs, punctuation, numbers, and special characters  
- Removes HTML tags  
- Removes unwanted patterns  

This cleaned text then goes into the TF-IDF vectorizer.

---

 Models Used

1. Logistic Regression**
- Works extremely well with high-dimensional, sparse text data  
- Fast and efficient  
- Great baseline model for text classification  
- Provided the best performance in this project  

2. Decision Tree Classifier**
- Captures non-linear relationships  
- Easy to interpret  
- Helpful for comparing linear and non-linear approaches  

Both models were evaluated to see how they behave on the same feature set.



Results

Logistic Regression performed better than the Decision Tree model.

Here is an example of how the results might look (replace with your actual numbers):

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 0.98 |
| Decision Tree | 0.92 |

---

## 📝 Manual Testing

The notebook includes a `manual_testing()` function that allows you to test custom news text:

```python
manual_testing("Your news article here")
# Fake-News-Detection1
