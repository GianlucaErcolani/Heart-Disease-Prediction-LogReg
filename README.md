# Heart Disease Prediction project

The goal of this project is to develop a machine learning classification model using **Logistic Regression** to predict the presence of heart disease in patients based on various clinical and demographic features. The project emphasizes robust data preprocessing, including categorical variable transformation and feature scaling, to ensure optimal model performance.

### Project Structure

* `Heart Disease UCI logistic regression.py`: Python script containing the complete workflow:
    * **Data Exploration (EDA)**: Inspection of dataset properties and visualization of numerical feature distributions using histograms.
    * **Feature Engineering**: Meaningful decoding of categorical variables (e.g., chest pain types, resting ECG, thalassemia types) followed by One-Hot Encoding (`get_dummies`) to prepare data for linear modeling.
    * **Data Preprocessing**: Application of `MinMaxScaler` to normalize continuous numerical features (such as Age, Blood Pressure, and Cholesterol) for stable Logistic Regression training.
    * **Predictive Modeling**: Implementation of a Logistic Regression classifier (`max_iter = 2000`) and evaluation using robust **5-fold cross-validation**.
* `requirements.txt`: List of Python libraries required to run the environment.

### Dataset

**Input variables (Clinical Markers):**
* `age`: Patient's age in years.
* `sex`: Patient's gender.
* `cp`: Chest pain type (asymptomatic, atypical angina, non-anginal pain, typical angina).
* `trestbps`: Resting blood pressure.
* `chol`: Serum cholesterol measurement.
* `fbs`: Fasting blood sugar.
* `restecg`: Resting electrocardiographic results (e.g., normal, ST-T wave abnormality, left ventricular hypertrophy).
* `thalach`: Maximum heart rate achieved during exercise.
* `exang`: Exercise-induced angina.
* `oldpeak`: ST depression induced by exercise relative to rest.
* `slope`: The slope of the peak exercise ST segment (downsloping, flat, upsloping).
* `ca`: Number of major vessels colored by fluoroscopy.
* `thal`: Thalassemia type (normal, fixed defect, reversable defect).

**Output variable (Target):**
* `target`: Presence of heart disease (binary classification).

### Results
The model's robustness and predictive accuracy were evaluated using **5-fold cross-validation** to ensure it generalizes well to unseen patient data, minimizing the risk of overfitting.
