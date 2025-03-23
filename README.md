# Classification of Tweets from Northern European Politicians  

## Overview  
This project classifies tweets from Northern European politicians into four political categories: **Left, Center, Right, and Independent** using supervised machine learning models. The best-performing model, **Linear Support Vector Classifier (SVC)**, achieved a **77.3% cross-validation accuracy** and **78.219% accuracy on Kaggle**.  

## Dataset  
The dataset includes tweets with the following key features:  
- `hashtags`: List of hashtags in the tweet  
- `full_text`: Tweet content (including emojis, HTML, hashtags)  
- `in_reply_to_screen_name`: Mentioned user (if any)  
- `country_user`: Country of the tweet owner  
- `pol_spec_user`: Political view (available only in training data)  

## Preprocessing  
- Removed **stopwords, emojis, punctuation, and links**  
- Applied **lemmatization** to normalize text  
- Extracted features using **TF-IDF and count-based methods**  

## Models Used  
The following models were tested:  
- **Linear SVC** 
- Logistic Regression  
- Random Forest

A **FeatureUnion** was used to combine different text feature extraction techniques.  

## Results  
- **Cross-validation accuracy**: **77.3%**  
- **Kaggle competition accuracy**: **78.219%**  
- **Challenges**: Misclassification in the **Independent category** due to class imbalance.  

## Topic Modeling  
To analyze common themes in tweets, the project applied:  
- **Latent Dirichlet Allocation (LDA)**  
- **Non-negative Matrix Factorization (NMF)**  

These models helped identify topics such as **political discussions, social issues, and global trends**.  


