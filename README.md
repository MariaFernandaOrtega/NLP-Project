# NLP Project
## Summary

One of the main challenges of the digital era is the difficulty of assessing the reliability of information sources. This project compares two machine learning models (Logistic Regression and Passive-agressive) to detect fake news in two languages: English and Spanish. The data was obtained from the "ISOT Fake News" database, made available by the University of Victoria, Canada, for the english news, and  by web scraping data from  news websites for the Spanish news.  The results in both languages show a lower level of logistic regression performance compared to the passive aggressive classifier. The metrics used to measure performance are Accuracy and F1 Score, in addition to the confusion matrix and cross-validation to ensure the absence of bias during the training and adjustment phase. 

## Proposed Method
<img width="487" alt="Screenshot 2023-03-30 165840" src="https://user-images.githubusercontent.com/112641687/228881981-4b7d56c3-f704-4362-b837-42c74c22ea91.png">

## Experimental details: 
For this project, two experiments have been carried out. The first one analyses the database with news in English and compares the results of the evaluation metrics on the title and the text of the news. Furthermore, the dataset was divided into training data (70%) and test data (30%). The selected models were set with default parameters.
For the second experiment, a new database with news in Spanish was selected to evaluate the quality of the models, Logistic Regression and Passive Aggressive, in detecting fake news using the text of the news, and compare it with the results obtained in the first experiment. In this case, the training data is 80% and the test data is 20%. First, the selected classifiers were set with the default parameters, and then a hyper-parameter tuning was performed for the model that obtained the lowest result (Logistic Regression).

## Results Experiment 1: 
The results related to this experiment can be divided into two levels of evaluation: data analysis time and classification quality in predicting fake news.

<img width="493" alt="Screenshot 2023-03-31 111042" src="https://user-images.githubusercontent.com/112641687/229078221-0887ec3c-cb4b-4d9f-b7c9-3b8130fc054d.png">


## Results Experiment 2: 
Table 3 provides an overview of the quantitative performance of the models in predicting fake news in Spanish. In this experiment, the passive-aggressive algorithm outperformed the logistic regression model with a F1-score of 92% and an Accuracy rate of 95%.


<img width="281" alt="Screenshot 2023-03-31 111316" src="https://user-images.githubusercontent.com/112641687/229079475-d68394b8-89dd-4c0d-bffe-77a3a00ffebe.png">

Furthermore, table 4 shows a comparison of the F1 Score between the articles in English (first experiment) and the news in Spanish. The results are significantly better when implementing the models on the English database.


<img width="392" alt="Screenshot 2023-03-31 111421" src="https://user-images.githubusercontent.com/112641687/229079516-ff2df2d6-0d5f-4e11-bd4b-652a64cf6610.png">


