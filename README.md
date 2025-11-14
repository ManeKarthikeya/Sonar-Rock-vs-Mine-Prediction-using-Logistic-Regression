# Sonar Rock vs Mine Prediction using Logistic Regression

## 📖 Project Overview

This project implements a Machine Learning classifier to distinguish between Rocks and Metal Cylinders (Mines) using sonar signal data. The model analyzes the energy returns from sonar signals bouncing off different objects to make its prediction.

It's a classic binary classification problem and serves as an excellent introduction to machine learning with real-world sensor data.

## 🧠 Algorithm Used

**Logistic Regression**: A fundamental and powerful linear model for binary classification tasks.

## 📊 About the Dataset

- The dataset contains 208 sonar signal samples.
- Each sample has 60 numerical features representing the energy within a particular frequency band, measured over a specific period.
- The target variable is a label: "R" for Rock or "M" for Mine.
- **Source**: The dataset is from kaggle.

## 🛠️ Implementation Steps

The code follows a standard machine learning pipeline:

1. **Import Dependencies**: Uses pandas, numpy, and scikit-learn.
2. **Data Loading & Exploration**: Loads the data and performs basic exploratory data analysis (EDA) to understand its structure.
3. **Data Preprocessing**: Separates the data into features (X) and labels (y).
4. **Train-Test Split**: Splits the data into training and testing sets, using stratification to maintain the class distribution.
5. **Model Training**: A Logistic Regression model is trained on the training data.
6. **Model Evaluation**: The model's performance is evaluated by calculating its accuracy on both the training and test sets.
7. **Prediction System**: A final script is provided to make a prediction on a new, single sonar reading.

## 📈 Results

The model's performance is evaluated based on its accuracy:

- **Training Accuracy**: The accuracy achieved on the data the model was trained on.
- **Test Accuracy**: The accuracy achieved on the unseen test data, which is a better indicator of real-world performance.

*(Note: The exact accuracy percentages will be displayed when you run the code.)*

## 🚀 How to Run this Project

1. **Clone the repository**:
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
```

2. **Navigate to the project directory**.

3. **Install the required libraries**:
```bash
pip install numpy pandas scikit-learn
```

4. **Prepare the dataset**:
   - Download the sonar.all-data CSV file from the UCI repository (or use the one provided if included).
   - Update the file path in the code: `sonar_data = pd.read_csv('path/to/your/sonar_data.csv', header=None)`

5. **Run the Python script**:
```bash
python sonar_rock_vs_mine_prediction_with_python.py
```

## 💡 Making a Prediction

To make a prediction on a new sonar reading, replace the `input_data` variable in the "Making a Predictive System" section with a list of 60 numerical values. The script will output whether the object is predicted to be a Rock or a Mine.

**Example:**
```python
input_data = (0.0307, 0.0523, 0.0653, 0.0521, 0.0611, 0.0577, 0.0665, 0.0664, 0.1460, 0.2792, ...) # ... must be 60 values
```

## 📁 Repository Structure

```
├── sonar_rock_vs_mine_prediction_with_python.py  # Main Python script
├── sonar_data.csv                                # Dataset (if included)
└── README.md                                     # Project description (this file)
```
