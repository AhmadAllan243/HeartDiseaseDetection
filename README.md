# HeartDiseaseDetection

## Description and Breakdown

Our project focuses on detecting heart diseases and predicting whether a patient might have a heart disease. We began by choosing a dataset that included 14 factors for us to interpret, they include:

- Age
  
- Sex
  
  -- Value 0: female

  -- Value 1: male

- Cp : chest pain type
  
- Trestbps: resting blood pressure
  
- Chol: serum cholesterol in mg/dl
  
- fbs: fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
  
- Restecg: resting electrocardiographic results
  
- Thalach: maximum heart rate achieved
  
- exang: exercise induced angina (1 = yes; 0 = no)
  
- Oldpeak: ST depression induced by exercise relative to rest
  
- Slope: the slope of the peak exercise ST segment
  
  -- Value 1: upsloping
  
  -- Value 2: flat
  
  -- Value 3: downsloping
- ca: number of major vessels (0-3) colored by fluoroscopy
  
- Thalassemia: blood disorder caused when the body doesn't make enough hemoglobin
  
  -- Value 3: normal
  
  -- Value 6: fixed defect
  
  -- Value 7: reversible defect
  
- Num: diagnosis of heart disease (predicted value)
  
  -- Value 0: < 50% diameter narrowing
  
  -- Value 1: > 50% diameter narrowing
  


The ‘num’ variable is the final output which detects whether a patient might have a heart disease or not. We faced a small problem with missing values in parts of the dataset but then decided to replace all missing values with NULL, then after having to fill up the NULL values to apply the algorithms, we calculated the mean of the the values that were already there and replaced the NULL values with the values we calculated. 

## Methedology

For our dataset, we first had to process the data in order to get rid of non-numerical values in any rows, as well as ensure that any missing values are represented correctly. To do so, we imported all necessary libraries as well as the dataset file as a csv. Then, we created columns where each respective value for each patient would fall under (age, sex, cp…). We also had missing values that were represented with question marks. In order to make it correctly insertable into the algorithms, we replaced all question marks with NA.

Then, we decided to use two algorithms for our models, Naive Bayes and Neural Network.

First, we used the naive Bayes algorithm in order to create a model which predicts whether patients could possibly have heart disease or not (where 0 represents unlikely to have heart disease, and 1 represents that they are prone to heart disease). This model was suitable because it categorically classifies data into groups, which was something essential to our dataset. 
For this algorithm we had to replace the missing values (previously filled as NA) with the mean of all other values in the same column, we did this to obtain a prediction, otherwise the algorithm was not able to ignore the NA values.

For the second algorithm we created a neural network. We chose this approach as we were curious how an algorithm designed for complex data such as this one would perform with relatively simple patient data. As it turns out, the Naive Bayes algorithm actually yielded more accurate results. We had to convert our values in the dataset to ‘float32’ or ‘int32’ in order for the values to be insertable into the algorithm.

Finally, we created representational graphs (ROCs) for both algorithms in order to make the analysis process simpler and more understandable. We also created a comparative bar graph in order to demonstrate the difference in accuracy between the two algorithms.

## Project Report

[Heart Disease Prediction.pdf](https://github.com/AhmadAllan243/HeartDiseaseDetection/files/13428831/Heart.Disease.Prediction.pdf)
