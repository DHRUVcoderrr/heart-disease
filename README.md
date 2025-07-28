# heart_diseases-prediction


```markdown
# Heart Disease Prediction

This project uses a Logistic Regression model to predict the likelihood of heart disease based on several health indicators. The dataset used for training and testing contains 303 instances with features such as age, sex, cholesterol levels, blood pressure, and more.

## Project Overview

The objective of this project is to build a classification model that predicts whether or not a person has heart disease based on their medical records.

- **Target Variable**: 
  - 0: Presence of heart disease.
  - 1: Absence of heart disease.
- **Features**: Age, sex, chest pain type (cp), resting blood pressure (trestbps), cholesterol (chol), fasting blood sugar (fbs), and others.

## Dataset

The dataset used in this project is the **Heart Disease Data**, which contains 303 records with 14 features (including the target variable).

### Columns:
- `age`: Age of the patient
- `sex`: Sex (1 = male; 0 = female)
- `cp`: Chest pain type (0-3)
- `trestbps`: Resting blood pressure
- `chol`: Serum cholesterol in mg/dl
- `fbs`: Fasting blood sugar (>120 mg/dl, 1 = true; 0 = false)
- `restecg`: Resting electrocardiographic results
- `thalach`: Maximum heart rate achieved
- `exang`: Exercise induced angina (1 = yes; 0 = no)
- `oldpeak`: ST depression induced by exercise
- `slope`: The slope of the peak exercise ST segment
- `ca`: Number of major vessels (0-4) colored by fluoroscopy
- `thal`: Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect)
- `target`: 1 = No heart disease, 0 = Heart disease

## Getting Started

### Prerequisites

- Python 3.x
- Libraries used: 
  - pandas
  - numpy
  - scikit-learn (LogisticRegression, accuracy_score, train_test_split, StandardScaler)
  
You can install the dependencies by running:

```bash
pip install -r requirements.txt
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/Ashwadhama2004/heart-disease-prediction.git
```

2. Navigate to the project directory:

```bash
cd heart-disease-prediction
```

3. Run the script:

```bash
python main.py
```

## Model

A **Logistic Regression** classifier is used for this project. The data is split into training and testing sets with 80% of the data used for training and 20% for testing.

- **Training Accuracy**: ~84.3%
- **Testing Accuracy**: ~80.3%

To improve model convergence, features are scaled using **StandardScaler**. The logistic regression model's solver is set to `lbfgs` and trained with default settings.

## Usage

You can run the provided script to fit the Logistic Regression model and make predictions.

```python
# Example of fitting the model
classo = LogisticRegression()
classo.fit(X_train, Y_train)
```

The script will output accuracy scores for both the training and testing datasets.

## Results

- **Training Accuracy**: 84.3%
- **Testing Accuracy**: 80.3%

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Example License Section:
You will also need to add an MIT license file to your repository. Here’s an example `LICENSE` file you can use:

```plaintext
MIT License

Copyright (c) 2024 [Gaurang Chaturvedi]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

You can copy these to your repository and make necessary adjustments like replacing `[Your Name]` and your GitHub username where appropriate.
