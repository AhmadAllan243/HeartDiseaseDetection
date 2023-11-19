# HeartDiseaseDetection

Our project focuses on detecting heart diseases and predicting whether a patient might have a heart disease. We chose a dataset that included 14 factors for us to interpret, they include:
Age
Sex
-- Value 0: female
-- Value 1: male
Cp : chest pain type
Trestbps: resting blood pressure
Chol: serum cholesterol in mg/dl
fbs: fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
Restecg: resting electrocardiographic results
Thalach: maximum heart rate achieved
exang: exercise induced angina (1 = yes; 0 = no)
Oldpeak: ST depression induced by exercise relative to rest
Slope: the slope of the peak exercise ST segment
-- Value 1: upsloping
-- Value 2: flat
-- Value 3: downsloping
ca: number of major vessels (0-3) colored by fluoroscopy 
Thalassemia: blood disorder caused when the body doesn't make enough hemoglobin
            -- Value 3: normal
 -- Value 6: fixed defect
 -- Value 7: reversible defect
Num: diagnosis of heart disease (predicted value)
-- Value 0: < 50% diameter narrowing
-- Value 1: > 50% diameter narrowing
The ‘num’ variable is the final output which detects whether a patient might have a heart disease or not. We faced a small problem with missing values in parts of the dataset but then decided to replace all missing values with NULL, then after having to fill up the NULL values to apply the algorithms, we calculated the mean of the the values that were already there and replaced the NULL values with the values we calculated. 
