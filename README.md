![alt text](https://kaggle2.blob.core.windows.net/competitions/kaggle/5039/media/kaggle_pets2.png)

# Kaggle Shelter Animal Outcome Project

The main goal of the project is to come up with a model that can predict the outcome of a shelter animal given some attributes such as species, color, age, whether it has a given name or not etc. Detailed description can be accessed [here](https://www.kaggle.com/c/shelter-animal-outcomes#description).

## Comment about the repository

The initial project was shared under ML_Project repository in my github. But I created a separate repository for cleaner presentation. Also, comments in the main jupyter notebook are written in Korean. I'll try and upload a verison with English comments ASAP.

## File Description

* Project_main.ipynb, Project_temp.ipynb - Initially, the final version was saved under Project_main.ipynb, but some rework was necessary and the final submission version is Project_temp.ipynb.

* Crawling Dog Breed Category.ipynb - We found and crawled some useful information on dog breeds on Google which we used to create new variables in the project.

* ML_project_joseph.ipynb, For_Presentation_6th.ipynb - These versions were used for the presentation given in the coding camp.

* train.csv, test.csv - These are data files provided by Kaggle and can be found in the data set hyperlink below in the Data and Evaluation Criteria section.

* Submission1 ~ Submission6.csv - These are the actual submission files to Kaggle.


## Data and Evaluation Criteria

* The data set is provided by Kaggle competition and can be found [here](https://www.kaggle.com/c/shelter-animal-outcomes/data).
* The evaluation criteria is log loss and more detail can be found [here](https://www.kaggle.com/c/shelter-animal-outcomes#evaluation).
* The leader scoreboard can be found [here](https://www.kaggle.com/c/shelter-animal-outcomes/leaderboard)

## Quick Summary

Several models, including Logistic Regression, Naive Bayesian, Random Forest, Extreme Forest and XGBoost, were utilized. For data preprocessing, we crawled animal size and ranking information and included them as variables. For the categorical variables, we used Pandas' get_dummies method which performs a clean one hot encoding. 

The final model was XGBoost with max_depth = 6 and n_estimators = 300. Our team score ranked around 540 out of 1600 competitors.

## Useful References

* [Kaggle Competition Description](https://www.kaggle.com/c/shelter-animal-outcomes)
* [Mixed Breed](http://www.vetstreet.com/our-pet-experts/can-you-predict-the-adult-size-of-a-mixed-breed-puppy) - Provides information on how to handle mixed breed.
* [Size Reference](http://www.dogbreedslist.info/herding-dog-breeds/#.WltQz6hl-iO) - This website provides useful information for breed to size conversion. We crawled a lot of information from this webpage to construct new variables.
* [Shelter Animal XGBoost Approach](https://nishadikirielle.wordpress.com/2016/10/08/kaggle-competition-shelter-animal-problem-xgboost-approach/) - This blog provides a good overview of XGBoost approach to solve the problem. It also provided a good tip on how the ranking of the dog breed can help improve the accuracy.
* [Some issues with Kaggle ranking](https://www.kaggle.com/c/shelter-animal-outcomes/discussion/22119) - Apparently there were some complex issues with result matching using data leak. A very important read

## Acknowledgments

This project was carried out a team project in Machine Learning session at FastCampus Data Science coding camp.

