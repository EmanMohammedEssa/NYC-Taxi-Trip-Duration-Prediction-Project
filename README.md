# NYC Taxi Trip Duration Prediction

## 📌 Project Overview
This project aims to predict the duration of NYC taxi trips using machine learning techniques. The dataset includes various trip details such as pickup and drop-off locations, timestamps, and other relevant features.

## 📂 Dataset
The dataset used in this project consists of NYC taxi trip records with features including:
- `pickup_datetime`: Timestamp of when the trip started.
- `dropoff_datetime`: Timestamp of when the trip ended.
- `passenger_count`: Number of passengers in the taxi.
- `pickup_longitude` & `pickup_latitude`: Pickup coordinates.
- `dropoff_longitude` & `dropoff_latitude`: Drop-off coordinates.
- `trip_duration`: Target variable (trip duration in seconds).

## 🔧 Preprocessing & Feature Engineering
Key preprocessing and feature engineering steps include:
- Handling missing values.
- Converting timestamps to useful time-based features (e.g., hour, weekday, etc.).
- Calculating the haversine distance between pickup and drop-off points.
- Removing outliers to improve model performance.

## 🚀 Model & Evaluation
A **Ridge Regression** model was used to predict trip duration. The evaluation metric for this project is the **R² score**, which achieved **85% accuracy**.

## 📊 Results & Insights
- The model performs well with an R² score of 0.85, indicating a strong correlation between the predicted and actual trip durations.
- Feature engineering, such as adding distance-based features, significantly improved model performance.
- Further improvements can be achieved by experimenting with advanced models like Gradient Boosting or Neural Networks.

## 📁 Project Structure
```
NYC-Taxi-Trip-Duration-Prediction-Project/
│── data/               # Contains dataset files
│── notebooks/          # Jupyter notebooks for EDA & model training
│── models/             # Saved trained models
│── src/                # Scripts for preprocessing & training
│── README.md           # Project documentation
```

## 🛠 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/EmanMohammedEssa/NYC-Taxi-Trip-Duration-Prediction-Project.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the preprocessing and training scripts:
   ```bash
   python src/preprocess.py
   python src/train_model.py
   ```
4. Evaluate the model:
   ```bash
   python src/evaluate.py
   ```

## 📜 License
This project is open-source and available under the MIT License.

---
📌 **Author:** [Eman Mohammed Essa](https://github.com/EmanMohammedEssa)
