# Wine-Quality-Analysis
Analytics on Quality Assessment through physio-chemical properties of Portuguese Wine

## Introduction
This notebook evaluates input variables and focuses to use Classification Tree to analyse Portuguese wine data and determine important predictors.  Further, Stepwise Linear Regression approach through Microsoft excel is employed to build a model to predict the quality of wine.

Source dataset: https://www.kaggle.com/abhishekmamidi/introduction-to-regression-complete-analysis

Oenology is the science and study of wine and winemaking. The analysis uses Portuguese wine, Vinho Verde (named after the same region) which is considered as a young wine because it is consumed fresh, after harvesting for merely 3-6 months. Broadly speaking, among different variants of wines two are worldwide popular by their names: Red wine and White wine. 
The 11 physiochemical properties predict the quality based on sensory results given by Sommeliers scored between 0-10. 

### The Report explains the following:
Understanding of the data by explaining wine properties generically speaking and how they relate with the taste of the final product. Further, intuitive relations and analysis results are explained.

### Python Notebook focuses on:
Feature selection through Classification Tree and includes Preprocessing, Train/test split , hyperparameter tuning and feature selection to compare the results of Excel Stepwise Regression Model

## Result
Both methods (random search and grid search CV) agree with the top 5 predictors. They are:
Alcohol, Sulphates, Total Sulphur dioxide, Volatile Acidity and Residual Sugar
The Stepwise Regression Model selects top three features as Alcohol, Volatile Acidity and Sulphur Di Oxide.

## Conclusion 
1.	More Alcohol is desired for a better quality- A widely accepted idea is that alcohol reduces the palatte sensitivity and therefore, lower alcohol wines are usually considered balanced which thus pair better with foods. However, it is interesting that when tasting wine, alcohol is well received due to the fact that in wines it tends to draw out more intense flavors. They are called fuller bodied wines. It is the most significant factor to determine the quality of wine. As per the analysis, for a wine sample if volatile acidity and sulfur dioxide which are significant in determining the quality (as per the equation) of wine are kept constant, one percent increase in volume of alcohol would increase the score by 0.65. For example, a quality score of 5 would go to 5.65 if percent by volume of alcohol increases from 9% to 10% . This demonstrates a very substantial raise in the quality.

2.	Result of acid- The second important factor for wine quality assessment is volatile acidity (acetic acid). Wines are perceived negatively (score reduces) when acid concentration increases because as expected, the acetic acid or vinegar flavour reduces the quality of a wine. This could also be due to the positive relation with pH level because acetic acid is one of the weak acid. 
Delving deeper into this, one expects an inverse relation between pH and acids. Although pH shows to have a negative correlation, i.e. inverse relation with fixed and citric acid as expected, it shows to have a positive one with volatile acidity. This is an unexpected result since acidity means lower pH values on the scale. Further research shows that volatile acidity usually means acetic acid which is a weak acid. Weak acid simultaneously contain their related base in one solution (https://en.wikipedia.org/wiki/Acid_strength#Conjugate_acid/base_pair). This possibly explains the positive correlation.

3.	Clean is tasty- Even though it makes sense that an antimicrobial compound would make the wine cleaner, it is a factor that hampers the quality of wine. This is understandable because this antimicrobial compound, sulfur dioxide, has a pungent repelling aroma which in more quantity results in lower quality level.






