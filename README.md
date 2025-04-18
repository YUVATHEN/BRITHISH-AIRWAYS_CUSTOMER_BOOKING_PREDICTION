# ✈️ British Airways Customer Booking Prediction

This machine learning project predicts whether a customer will complete a flight booking with British Airways based on travel preferences, booking channels, and flight details. The goal is to enhance customer conversion by identifying key behavioral indicators.

## 📂 Dataset Overview
The dataset includes information on passenger booking behavior and preferences:
- `Num_Passengers`: Number of passengers in the group  
- `sales_channel`: Booking platform (e.g., online, travel agent)  
- `trip_type`: Type of journey (RoundTrip, Oneway, CircleTrip)  
- `length_of_stay`: Duration at the destination  
- `Flight_day` / `Flight_hour`: Day and time of flight  
- `Route`, `booking_origin`, `Flight_duration`: Travel route and booking origin  
- Customer preferences:  
  - `wants_extra_baggage`  
  - `wants_preferred_seat`  
  - `wants_in_flight_meals`  
- Target variable: `booking_complete` (Yes/No)

## 🧹 Data Preprocessing
- Handled duplicates with domain logic consideration  
- Treated missing values and standardized categorical data  
- Performed label encoding for binary features  
- One-hot encoded multi-category variables like `sales_channel` and `trip_type`

## 📊 Exploratory Data Analysis (EDA)
- Analyzed booking patterns across `trip_type`, `sales_channel`, and `Route`  
- Observed higher booking completion among passengers who prefer in-flight services  
- Booking trends varied significantly with country of origin and day of travel

## ⚙️ Model Building
Several classification algorithms were tested:
- Logistic Regression  
- Decision Tree  
- Random Forest  
- XGBoost  

## 🏆 Best Model
- **XGBoost Classifier** provided the highest accuracy and performance  
- Metrics used: Accuracy, Precision, Recall, F1 Score  
- Feature importance revealed key predictors: `sales_channel`, `trip_type`, and service preferences

## 📌 Key Insights
- Customers preferring extras like meals and seats are more likely to complete bookings  
- Online sales channels showed higher conversion rates  
- Round-trip bookings had higher confirmation probabilities than one-way or circle trips

