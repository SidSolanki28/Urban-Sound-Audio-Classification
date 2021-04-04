#  Urban Sound Audio Classification

---

## Project Overview

- Objective : 
  - **To classifiy urban sound**
- Classification Problem
- Data cleaning
- Exploratory Data Analysis
- Data Preprocessing
- **Artificial Neural Network (ANN)** Training and Prediction

---
## About Project

Automatic environmental sound classification is a growing area of research with numerous real world applications. Whilst there is a large body of research in related audio fields such as speech and music, work on the classification of environmental sounds is comparatively scarce.

There is a plethora of real world applications for this research, such as:
• Content-based multimedia indexing and retrieval
• Assisting deaf individuals in their daily activities
• Smart home use cases such as 360-degree safety and security capabilities
• Industrial uses such as predictive maintenance

---
## Code and Resources used

- Python version: 3.7.6
- Packages: Pandas, Numpy, Seaborn, Matplotlib, Scikit, Keras, Tensorflow, Librosa, Ipython
- Resources used:

* Medium : https://mikesmales.medium.com/sound-classification-using-deep-learning-8bc2aa1990b7
* Heartbeat : https://heartbeat.fritz.ai/working-with-audio-signals-in-python-6c2bd63b2daf

---
## Web Scraping

Dataset URL: https://urbansounddataset.weebly.com/urbansound8k.html

For this we will use a dataset called Urbansound8K. The dataset contains 8732 sound excerpts (<=4s) of urban sounds from 10 classes, which are:
• Air Conditioner
• Car Horn
• Children Playing
• Dog bark
• Drilling
• Engine Idling
• Gun Shot
• Jackhammer
• Siren
• Street Music

---
## Data Cleaning

There is no missing values in data.

---
## EDA

I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights :

![](https://github.com/SidSolanki28/Absenteeism-at-Work/blob/master/Images/download%20(1).png)
![](https://github.com/SidSolanki28/Absenteeism-at-Work/blob/master/Images/download%20(2).png)

---
## Model Building

### Logistic Linear Regression

Logistic regression is named for the function used at the core of the method, the logistic function.
Below is an example logistic regression equation:

y = e^(b0 + b1*x) / (1 + e^(b0 + b1*x))

Where y is the predicted output, b0 is the bias or intercept term and b1 is the coefficient for the single input value (x). Each column in your input data has an associated b coefficient (a constant real value) that must be learned from your training data.

The logistic function, also called the sigmoid function

---
## Model Prediction

| Features| Coefficients | Odds Ratio 
| ----------- | ----------- | --------- |
| Reason C | 1.716629 | 5.565735 |
| Reason A | 1.559403 | 4.755983 |
| Transportation expense	| 0.701718	| 2.017215 |
|	Social drinker | 0.588378	| 1.801065 |
|	Weight	| 0.586728 | 1.798096 | 

---
## Model Performance

| Label | precision | recall |  f1-score 
| ----------- | ----------- | --------- | ------- |
| 0 | 0.81 | 0.77 | 0.79 |
| 1 | 0.69 | 0.74 | 0.72 |
| accuracy |  |   | 0.76 |    

## Conclusion

After analyzing its Odd Ratios and Coefficients, we predict

- Reason A and C has most weightage

Therefore, reasons like poisoning, injuries and various diseases are most common reasons for absenteeism.

- Also, Transport is also an issue for an employee to get absent for hours.

- Also, Disciplinary failure has highly negative coefficient means if there is no discipine penalty, there is more chance that employee become present in working hours.

---

## Further Improvements

Working on SQL and Tableau Integration
