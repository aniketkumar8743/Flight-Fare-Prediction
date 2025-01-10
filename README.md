# 🚁 Flight Fare Prediction

## 📊 Overview
The **Flight Fare Prediction** project aims to build a machine learning model to predict the price of flight tickets based on various features such as departure time, arrival time, duration, and other flight-specific details. Accurate prediction of flight fares can help customers make informed decisions and airlines optimize pricing strategies.

## 🎯 Project Goal
The primary objective of this project is to develop a predictive model using the **Random Forest** algorithm to estimate flight fares. To enhance the model's performance, **Randomized Search Cross-Validation** was applied for hyperparameter tuning, resulting in a final accuracy of **84.22%**.

---

## 📈 Dataset
The dataset used for this project contains details about flights, including:
- Airline
- Date of Journey
- Source
- Destination
- Route
- Duration
- Total Stops
- Additional Info
- Price (target variable)

### 🗃️ Data Source
The dataset was sourced from [mention source, e.g., Kaggle, open datasets, or collected manually].

### 🔄 Data Preprocessing
- Handled missing values.
- Converted categorical data into numerical form using techniques like **One-Hot Encoding** and **Label Encoding**.
- Extracted features like:
  - Departure time (hour)
  - Arrival time (hour)
  - Journey day and month.
- Standardized numerical features to improve model performance.

---

## 🔢 Data Analysis
Exploratory Data Analysis (EDA) was performed to understand the dataset better:
- Visualized relationships between features and the target variable (price) using **matplotlib** and **seaborn**.
- Checked feature importance to identify the most influential predictors.
- Analyzed correlations between numerical features.

---

## 📊 Model Training
1. **Algorithm Used**: Random Forest Regressor
2. **Why Random Forest?**
   - Handles non-linear relationships well.
   - Reduces overfitting by averaging multiple decision trees.
   - Provides feature importance insights.
3. **Hyperparameter Tuning**:
   - Applied **Randomized Search Cross-Validation** to find optimal parameters such as:
     - Number of estimators (n_estimators)
     - Maximum depth (max_depth)
     - Minimum samples split (min_samples_split)
     - Minimum samples leaf (min_samples_leaf)

---

## 🏆 Results
- **Model Accuracy**: 84.22%
- The model demonstrates good predictive performance on test data.
- Feature importance analysis revealed key factors influencing flight fares:
  1. Airline
  2. Duration
  3. Total Stops
  4. Source and Destination

---

## 🛠️ Usage
### 🔧 How to Use the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/username/flight-fare-prediction.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook or script to preprocess the data and train the model.
4. Use the trained model to make predictions by providing flight details as input.

### 🔢 Example Prediction
Input:
- Airline: Indigo
- Date of Journey: 2023-12-25
- Source: Delhi
- Destination: Mumbai
- Total Stops: 1
- Duration: 2h 30m

Output:
- Predicted Fare: ₹4,500

---

## 🔬 File Structure
```
flight-fare-prediction/
├── data/
│   ├── flight_data.csv
├── notebooks/
│   ├── EDA.ipynb
│   ├── model_training.ipynb
├── src/
│   ├── preprocessing.py
│   ├── model.py
├── results/
│   ├── evaluation_metrics.txt
│   ├── feature_importance.png
├── README.md
├── requirements.txt
```

---

## 📊 Tools and Libraries
- **Programming Language**: Python
- **Libraries Used**:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn

---

## 🚀 Future Enhancements
1. Incorporate additional features such as seasonality and demand trends.
2. Deploy the model using **Flask** or **Streamlit** for real-time predictions.
3. Optimize preprocessing steps for faster execution.

---



---

## ❤️ Acknowledgments
- Dataset sourced from [mention source].
- Inspired by flight pricing challenges and machine learning applications.

---

Feel free to contribute to this project by submitting issues or pull requests!

