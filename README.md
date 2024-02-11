

# AI Drug Classification Model

## Overview
This repository contains code for building a machine learning model to classify drugs based on patient data. The model utilizes various features such as age, sex, blood pressure, and cholesterol levels to predict the appropriate drug for a patient.

## Dataset
The dataset used for training and testing the model is stored in `drug200.csv`. It includes the following columns:

- Age: Age of the patient.
- Sex: Gender of the patient (Categorical: 'M' for male, 'F' for female).
- BP: Blood pressure level (Categorical: 'LOW', 'NORMAL', 'HIGH').
- Cholesterol: Cholesterol level (Categorical: 'NORMAL', 'HIGH').
- Na_to_K: Sodium to potassium ratio.
- Drug: Target variable indicating the prescribed drug (Categorical: 'drugA', 'drugB', 'drugC', 'drugX', 'drugY').

## Workflow
1. **Data Exploration**: The dataset is explored to understand its structure and characteristics. Summary statistics and visualizations are used to gain insights into the distribution of features and the target variable.

2. **Preprocessing**: Non-numerical columns ('Sex', 'BP', 'Cholesterol', 'Drug') are encoded into numerical format using Label Encoding. Numerical features are standardized using StandardScaler.

3. **Model Selection and Training**: A Random Forest Classifier is chosen as the model for drug classification. The model is trained on the preprocessed data.

4. **Hyperparameter Tuning**: Grid Search Cross Validation is performed to fine-tune the hyperparameters of the model and improve its performance.

5. **Model Evaluation**: The trained model is evaluated on a separate test set using metrics such as accuracy and classification report to assess its performance in drug classification.

## Dependencies
- Python 3.x
- pandas
- scikit-learn
- matplotlib

## Usage
1. Clone the repository:
   ```
   git clone https://github.com/your_username/ai-drug-classification.git
   ```
2. Navigate to the project directory:
   ```
   cd ai-drug-classification
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Run the main script:
   ```
   python drug_classification.ipynb
   ```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

You can customize this README file further by adding more details or sections as needed. Make sure to replace placeholders like Shiavnshraj567 with your actual GitHub username and adjust paths or commands accordingly.
