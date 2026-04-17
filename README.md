# -Duplicate-Question-Detection-using-NLP-Techniques-TF-IDF-and-BERT-
A Natural Language Processing project that detects whether two questions are semantically similar using TF-IDF and BERT
Duplicate Question Detection using NLP (TF-IDF & BERT)
## Overview

This project focuses on detecting whether two questions have the same meaning, even if they are phrased differently. Duplicate questions are common in platforms like Quora and can negatively impact search efficiency and user experience.

The project uses both traditional NLP techniques (TF-IDF) and advanced deep learning models (BERT) to compare their effectiveness in identifying duplicate questions.

## Objective
* Build a model to classify question pairs as duplicate or not duplicate

* Improve semantic understanding of text using modern NLP techniques

* Compare baseline and advanced approaches

## Dataset

The dataset contains:

-question1 – First question

-question2 – Second question

-is_duplicate – Target label (1 = duplicate, 0 = not duplicate)

 ## Project Workflow
1. Data Preprocessing

-Removed missing values

-Converted text to lowercase

-Removed numbers and punctuation

-Applied text cleaning functions

2. Feature Engineering

-Question length (q1_len, q2_len)

-Length difference

-Common word count

-Combined question text

3. TF-IDF Vectorization

-Used TfidfVectorizer (max_features=5000)

-Converted text into numerical features

4. Model Training (Baseline)

-Model: Logistic Regression

-Train-test split: 80/20

-Combined sparse and numerical features

5. Evaluation

-Accuracy: 77.21%

-Metrics: Precision, Recall, F1-score
## Advanced Approach: BERT

-Used BERT (bert-base-uncased) from Transformers

-Captures semantic meaning and context

-Improves performance on complex sentence structures

## Key Insights

-TF-IDF works well for basic similarity detection

-It fails in capturing context and semantics

-BERT significantly improves semantic understanding

-Advanced models are better for real-world NLP problems

## Technologies Used

-Python

-NumPy, Pandas

-Scikit-learn

-Transformers (Hugging Face)

-PyTorch

## Future Improvements

-Fine-tune BERT for higher accuracy

-Use advanced models like RoBERTa or DistilBERT

-Deploy as a web application (Flask/Streamlit)

## Conclusion

This project developed a duplicate question detection system using both traditional and advanced NLP techniques. Initially, a baseline model was built using TF-IDF and Logistic Regression, which achieved good performance by capturing basic textual similarity. However, it showed limitations in understanding semantic meaning.

To overcome this, a BERT-based model was applied, which improved the ability to understand contextual and semantic relationships between questions. This resulted in better identification of duplicate questions, even when they were phrased differently.

Overall, the project demonstrates that while TF-IDF is efficient and useful for baseline modeling, BERT provides more accurate results by capturing deeper language understanding. This highlights the importance of using advanced transformer-based models for solving real-world NLP problems.
