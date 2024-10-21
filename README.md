# BREAST CANCER DETECTION
## About Dataset:
### Description:
Breast cancer is the most common cancer among women worldwide, accounting for approximately 25% of all cancer cases in women. In 2022, there were an estimated 2,296,840 new cases of breast cancer among women according to [World Cancer Research Fund International](https://www.wcrf.org/cancer-trends/breast-cancer-statistics/#:~:text=Breast%20cancer%20is%20the%202nd,was%20not%20reported%20for%20men.). It starts when cells in the breast begin to grow out of control. These cells usually form tumors that can be seen via X-ray or felt as lumps in the breast area.
The key challenge against its detection is classifying tumors into malignant (cancerous) or benign(non-cancerous).

### Acknowledgements:
This dataset has been referred from Kaggle

### Objective:
- Understand the Dataset & cleanup (if required).
- Build classification models to predict whether the cancer type is Malignant or Benign.
- Also fine-tune the hyperparameters & compare the evaluation metrics of various classification algorithms.

### Columns:
Note: se = (Standard Error) <br>
- ID number:
- Diagnosis: (M = malignant, B = benign)
- radius_mean: Radius of Lobes
- texture_mean: Mean of Surface Texture
- perimeter_mean: Outer Perimeter of Lobes
- area_mean: Mean Area of Lobes
- smoothness_mean: Mean of Smoothness Levels
- compactness_mean: Mean of Compactness
- concavity_mean: Mean of Concavity
- concave points_mean: Mean of Cocave Points
- symmetry_mean: Mean of Symmetry
- fractal_dimension_mean: Mean of Fractal Dimension
- radius_se: se radius
- texture_se: se of Surface Texture
- perimeter_se: Perimeter of se
- area_se: Area of se
- smoothness_se: se of Smoothness Levels
- compactness_se: se of Compactness
- concavity_se: se of Concavity
- concave points_se: se of Cocave Points
- symmetry_se: se of Symmetry
- fractal_dimension_se: se of Fractal Dimension
- radius_worst: worst radius
- texture_worst: worst Surface Texture
- perimeter_worst: worst perimeter
- area_worst: worst area
- smoothness_worst: worst Smoothness Levels
- compactness_worst: worst Compactness
- concavity_worst: worst Concavity
- concave points_worst: worst Cocave Points
- symmetry_worst: worst Symmetry
- fractal_dimension_worst: worst Fractal Dimension

## Key Insights
- 63% of the values present in the diagnosis column are benign.
- Most of the data are not normally distributed with a skewness that tends to the right. we can also see a lot of outliers in the dataset
- Because there is a statistically significant difference between Cancerous tumors and non_cancerous tumors after performing statistical tests, we can say:
  - Cancerous tumors have the highest mean radius lobes, mean outer perimeter of lobes, the mean area of lobes
  - Cancerous tumors are more compact and concave 
  - the null hypothesis could not be rejected so we can say that there is no difference between the mean of fractal dimension, the texture standard error, and the smoothness standard error of the cancerous and the non-cancerous tumors.
- SVM provided the best model with a precision score of 100%
- texture mean, concavity mean, fractal dimension standard error, worst Concavity, and Mean of Symmetry were the five most important features that helped in the predictions.
