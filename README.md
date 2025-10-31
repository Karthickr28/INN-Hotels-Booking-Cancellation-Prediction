# 🏨 INN Hotels Booking Cancellation Prediction

## 📘 Project Overview

The INN Hotels Group, a chain of hotels in Portugal, has been facing a significant rise in booking cancellations and no-shows. These cancellations result in major revenue losses, especially for last-minute bookings.  

To address this, we developed a **Machine Learning–based predictive model** to forecast which bookings are likely to be canceled. This helps the hotel group take proactive measures — such as modifying refund policies, optimizing overbooking strategies, and improving revenue management.

---

## 🎯 Business Objective

The project aims to:
- Identify key factors that influence booking cancellations.  
- Build a predictive model to **classify future bookings** as likely to be canceled or not.  
- Provide **data-driven recommendations** to minimize revenue loss and improve operational efficiency.

---

## 📊 Business Impact of Cancellations

Booking cancellations affect hotels in several ways:

1. 💸 **Revenue loss** when rooms go unsold.
2. 💰 **Higher costs** due to commission or advertising on distribution channels.
3. 🏷️ **Reduced profit margins** from last-minute discounts.
4. 👩‍💼 **Increased workload** on staff to manage cancellations and rebookings.

---

## 📂 Dataset Description

The dataset contains booking-related details for customers of INN Hotels Group.  
Each record represents one booking and includes demographic, transactional, and behavioral attributes.

| **Feature** | **Description** |
|--------------|----------------|
| `Booking_ID` | Unique identifier for each booking |
| `no_of_adults` | Number of adults |
| `no_of_children` | Number of children |
| `no_of_weekend_nights` | Weekend nights booked/stayed |
| `no_of_week_nights` | Weeknights booked/stayed |
| `type_of_meal_plan` | Meal plan chosen (None, Breakfast, Half board, Full board) |
| `required_car_parking_space` | Whether parking space was required (0/1) |
| `room_type_reserved` | Encoded room type reserved |
| `lead_time` | Days between booking and arrival |
| `arrival_year` | Year of arrival |
| `arrival_month` | Month of arrival |
| `arrival_date` | Day of month |
| `market_segment_type` | Source of booking (e.g., Online, Corporate, etc.) |
| `repeated_guest` | Whether the guest is a returning customer (0/1) |
| `no_of_previous_cancellations` | Count of past cancellations by the guest |
| `no_of_previous_bookings_not_canceled` | Count of successful bookings |
| `avg_price_per_room` | Average daily room price (in euros) |
| `no_of_special_requests` | Number of special room requests |
| `booking_status` | Target variable — whether the booking was canceled (Yes/No) |

---

## 🔍 Exploratory Data Analysis (EDA)

The following key business questions were explored during EDA:

1. **What are the busiest months for the hotel?**  
   → Helps identify seasonal trends and peak demand periods.

2. **Which market segment do most guests come from?**  
   → Insights into major booking channels and potential partnerships.

3. **How do room prices vary across market segments?**  
   → Understanding pricing sensitivity among different customer types.

4. **What percentage of bookings are canceled?**  
   → Quantifying the overall cancellation rate.

5. **Do repeating guests cancel more or less often?**  
   → Assessing brand loyalty and customer trust.

6. **Do special requests influence cancellations?**  
   → Evaluating operational handling and guest satisfaction.

---

## ⚙️ Machine Learning Pipeline

**Steps followed:**
1. **Data Preprocessing**
   - Handling missing values  
   - Encoding categorical variables  
   - Scaling numerical features  
   - Train-test split  

2. **Exploratory Data Analysis (EDA)**
   - Univariate & bivariate visualizations  
   - Correlation heatmaps  
   - Outlier detection  

3. **Model Building**
   - Logistic Regression  
   - Random Forest Classifier  
   - Gradient Boosting (XGBoost/LightGBM)  
   - Evaluation using accuracy, precision, recall, F1-score, ROC-AUC  

4. **Model Selection**
   - Best-performing model chosen based on validation metrics.  

5. **Feature Importance Analysis**
   - Identified key drivers such as `lead_time`, `avg_price_per_room`, and `previous_cancellations`.

---

## 🧠 Insights

- **High lead time** strongly correlates with cancellation probability.  
- **Repeat guests** are significantly **less likely** to cancel.  
- **Higher room prices** tend to increase the likelihood of cancellation.  
- **Market segment** plays a key role — online bookings see more cancellations than corporate ones.  
- Guests with **special requests** generally show a **lower cancellation rate** (possible indicator of intent to stay).

---

## 🧩 Tech Stack

- **Language:** Python 🐍  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost  
- **IDE/Notebook:** Jupyter Notebook / Google Colab  
- **Version Control:** Git & GitHub  
- **Visualization:** Matplotlib, Seaborn  

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/inn-hotels-cancellation-prediction.git
