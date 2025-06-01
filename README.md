# ✈️ Airline Passenger Satisfaction ML Project ✈️

## 🔍 Overview

Welcome to the Airline Passenger Satisfaction Project! In the highly competitive airline industry, understanding what makes a passenger satisfied is critical to business success. This project leverages the power of machine learning to predict passenger satisfaction — whether a traveler is "Satisfied" or "Neutral/Unhappy" — based on a wide array of travel-related and service-oriented features. By decoding the drivers of customer sentiment, airlines can boost service quality, target improvements, and retain loyal flyers. 🛫💡

---

## 🎯 Project Objective

- Predict passenger satisfaction using demographic, travel, and service-related features.
- Provide actionable insights for better decision-making and customer segmentation.

---

## 🧠 Business Goals

- ✅ Improve overall customer experience by identifying key pain points.
- ✅ Predict satisfaction levels to proactively address service issues.
- ✅ Segment customers based on likelihood of satisfaction for targeted service enhancements.

---

## 🛠️ Technologies Used

- **Python**: The driving force behind the code.
- **Jupyter Notebook**: For exploratory data analysis and model training.
- **pandas & NumPy**: For seamless data handling and numerical operations.
- **matplotlib & seaborn**: To visualize patterns and insights.
- **scikit-learn**: A suite of ML algorithms and tools.
- **XGBoost**: For high-performance gradient boosting. ⚡

---

## 📊 Dataset Overview

The dataset contains information on passengers’ travel experiences, demographics, and service ratings. Here's a snapshot of the key features:

| Column                 | Description                                                                                 |
| ---------------------- | ------------------------------------------------------------------------------------------- |
| `ID`                   | Unique passenger identifier                                                                 |
| `Gender`               | Female or Male                                                                              |
| `Age`                  | Passenger’s age                                                                             |
| `Customer Type`        | First-time or Returning                                                                     |
| `Type of Travel`       | Business or Personal                                                                        |
| `Class`                | Economy, Economy Plus, or Business                                                          |
| `Flight Distance`      | Distance flown in miles                                                                     |
| `Departure Delay`      | Delay at departure (in minutes)                                                             |
| `Arrival Delay`        | Delay at arrival (in minutes)                                                               |
| `Service Ratings`      | Ratings from 1 to 5 on booking ease, cleanliness, entertainment, food, WiFi, etc. (0 = N/A) |
| `Overall Satisfaction` | **Target variable** – Satisfied or Neutral/Unhappy                                          |

---

## ⚙️ Steps Taken

1. **Data Cleaning**

   - Handled missing values.
   - Converted target labels to binary values (1 = Satisfied, 0 = Neutral/Unhappy).

2. **Exploratory Data Analysis (EDA)**

   - Identified key patterns like class preference, delay impact, and service quality correlation with satisfaction.

3. **Preprocessing**

   - Encoded categorical variables.
   - Scaled numerical variables.

4. **Model Building**  
   Tested several models to find the best performer:

   - Logistic Regression
   - K-Nearest Neighbors (KNN)
   - Decision Tree 🌳
   - Random Forest
   - XGBoost 🚀
   - AdaBoost
   - Gradient Boosting

5. **Model Evaluation**
   - Compared models using **Accuracy**,**Confusion Matrix**
   - Plotted the ROC curve for all the models.

---

## 🏆 Best Model: XGBClassifier

After experimenting with multiple algorithms, the **XGBoost** classifier delivered the best performance on both training and testing datasets.

### 🔍 Why XGBoost?

- Handles both numerical and categorical features efficiently (after encoding).
- Robust to outliers and multicollinearity, which is common in customer feedback datasets.
- Automatically handles missing values (treats them as part of the learning process).
- Boosting framework helps it reduce bias and variance, making it better than a single decision tree.
- Built-in regularization (L1 & L2) helps prevent overfitting — important when there are many correlated service features.

## 🔧 How to Run the Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/airline-passenger-satisfaction-ml-project.git
   cd airline-passenger-satisfaction-ml-project
   ```
