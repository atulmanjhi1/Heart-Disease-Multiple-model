# Heart Disease Prediction using Random Forest

This project uses a machine learning model to predict the presence of heart disease based on patient data. The model is trained using the Random Forest algorithm and evaluates performance with accuracy, confusion matrix, and classification reports.

## Dataset

The dataset used for this project contains various health-related attributes of patients. The target variable is `HeartDisease`, which indicates whether the patient has heart disease or not.

### Dataset Columns:
- **Age**: Age of the patient
- **Sex**: Gender (1 = Male, 0 = Female)
- **ChestPainType**: Type of chest pain (encoded as categorical codes)
- **RestingBP**: Resting blood pressure
- **Cholesterol**: Serum cholesterol in mg/dl
- **FastingBS**: Fasting blood sugar (> 120 mg/dl, 1 = True, 0 = False)
- **RestingECG**: Resting electrocardiogram results (encoded as categorical codes)
- **MaxHR**: Maximum heart rate achieved
- **ExerciseAngina**: Exercise-induced angina (1 = Yes, 0 = No)
- **Oldpeak**: ST depression induced by exercise relative to rest
- **ST_Slope**: Slope of the peak exercise ST segment (encoded as categorical codes)
- **HeartDisease**: Target variable (1 = Heart disease, 0 = No heart disease)

## Dependencies

To run this project, you need the following libraries:
- pandas
- scikit-learn

## Steps

1. **Data Preprocessing**
   - Mapped categorical variables to numerical values:
     - `Sex`: Mapped 'M' to 1 and 'F' to 0.
     - `ChestPainType`, `RestingECG`, and `ST_Slope` were encoded using categorical codes.
     - `ExerciseAngina`: Mapped 'Y' to 1 and 'N' to 0.

2. **Splitting the Data**
   - The dataset was split into training and testing sets using an 80/20 ratio with `train_test_split()`.

3. **Model Training**
   - The **RandomForestClassifier** was used to train the model on the training set.

4. **Prediction**
   - The trained model was used to predict heart disease on the test set.

5. **Evaluation**
   - Model performance was evaluated using:
     - **Accuracy**: The proportion of correctly predicted labels.
     - **Confusion Matrix**: To visualise the performance of the classification.
     - **Classification Report**: Detailed report with precision, recall, and F1-score.
 


