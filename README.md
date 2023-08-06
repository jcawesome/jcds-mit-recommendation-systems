# Netflix Movie Recommendation
## Introduction
In this notebook, I will try and use different techniques I have learned from the **Recommendation Systems** course under the MIT - "Data Science and Machine Learning: Making Data-Driven Decisions" Program.

## Business Case
**Context:** 
> Online streaming platforms like Netflix have plenty of movies in their repository and if we can build a Recommendation System to recommend relevant movies to users, based on their historical interactions, this would improve customer satisfaction and hence, it will also improve the revenue of the platform. The techniques that we will learn here will not only be limited to movies, it can be any item for which you want to build a recommendation system.

Online streaming platforms like Netflix have plenty of movies in their repository and if we can build a Recommendation System to recommend relevant movies to users, based on their historical interactions, this would improve customer satisfaction and hence, it will also improve the revenue of the platform. The techniques that we will learn here will not only be limited to movies, it can be any item for which you want to build a recommendation system.

**Problem:** Building various recommendation systems using the `ratings` dataset:
* Knowledge/Rank based recommendation system
* Similarity-Based Collaborative filtering
* Matrix Factorization Based Collaborative Filtering


The notebook is divided into different sections:
* Data Dictionary
* Import Libraries
* Create Recommendation System
	* Model 1: Rank-Based Recommendation System
	* Model 2: User based Collaborative Filtering Recommendation System
	* Model 3: Item based Collaborative Filtering Recommendation System
	* Model 4: Matrix Factorization using SVD
	
* Summary

## Summary
In this case study, I saw three different ways of building recommendation systems. After tuning, here are the results:
* rank-based using averages (uses only rank to recommend movies)
* similarity-based collaborative filtering
	* user-based collaborative filtering (RMSE: 0.9571)
	* item-based collaborative filtering (RMSE: 0.9433)
* model-based (matrix factorization) collaborative filtering (RMSE: 0.8953)
> The above results show that finely-tuned user-based collaborative filtering produces the best predictive results for movie recommendations using the `ratings` dataset.
I also understood advantages/disadvantages of these recommendation systems and when to use which kind of recommendation systems.

## Future Improvements
This project assessment involves breaking down the analysis thru a series of questions. To further improve on this notebook, I should do the following:
* (Apply the models by using A/B Testing to measure the effectiveness of these systems)[https://aws.amazon.com/blogs/machine-learning/using-a-b-testing-to-measure-the-efficacy-of-recommendations-generated-by-amazon-personalize/]
