# Gupta_DuplicateQuestionDetection

## Introduction
 In today’s digital age, where information is readily available at our fingertips, question
 and answer platforms have become increasingly popular. Quora is one of the popular
 platforms where users can ask questions and receive answers from a diverse commu
 nity. Over 100 million people visit Quora every month, so it’s no surprise that
 people ask similar-worded questions. Multiple questions with the same intent can
 cause seekers to spend more time finding the best answer to their question, and make
 writers feel they need to answer multiple versions of the same question. Quora up
 loaded a competition on Kaggle where users were challenged to tackle the problem
 of duplicate questions having different threads.
 This project aims to detect duplicate question pairs on Quora by utilizing the
 power of machine learning techniques. The main aim of the project is to develop
 a model capable of accurately identifying and classifying duplicate question pairs.

 ## Preprocessig
 - Replacement of Special Characters
 - Pattern Replacement
 - Numerical Conversion
 - Decontracting Words
 - Removing HTML Tags
 - Removing Punctuations

## Feature engineering
- q1 len,q2_len
- q1 num words,q2 num words
-  word common
-  word total
-  word share
-  Token Features-cwc min,cwc max,csc min,csc max,ctc min,ctc max,lastword eq,firstword eq
-  Fuzzy Features-fuzz ratio,fuzz partial ratio,token sort ratio,token set ratio


 ## Model Used
 - RandomForest
 - Xgboost
 - Naive Bayes
 - Logistic regression

## Result

 From the below Model results it is clear that our two best models are XGboost
 with an accuracy of 76.73 and RandomForest with an accuracy of 76.69. According
 to accuracy, the XGBoost and RandomForest almost gives the same result.
![Alt text](https://github.com/Gpriti/Gupta_DuplicateQuestionDetection/blob/main/model_comparasion.png)

## References
1. [FuzzyWuzzy](https://chairnerd.seatgeek.com/fuzzywuzzy-fuzzy-string-matching-in-python/)
2. [RandomForest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
3. [naiveBayes](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html)
4. [[LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)

