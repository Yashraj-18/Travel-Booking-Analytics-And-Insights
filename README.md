# Travel Booking Analytics

End-to-end analysis of hotel booking demand data using Python (Pandas, NumPy) and SQL (SQLite) to uncover patterns in cancellations, pricing dynamics, lead times, and seasonal demand for an OTA-style platform.

---

## 🛠️ Tools & Technologies
- **Python**: Pandas, NumPy
- **Database / SQL**: SQLite (in-memory execution via Python/Pandas)
- **Environment**: Jupyter Notebook / Google Colab / VS Code

---

## 📊 Dataset
- **Name**: Hotel Booking Demand Dataset ([Kaggle Link](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand))
- **Records**: 119,390 bookings across Resort Hotel (H1) and City Hotel (H2)
- **Features**: 32 columns (booking dates, lead time, customer types, ADR, cancellation status, room types, etc.)

---

## 💡 Key Insights

1. **Overall Cancellation Rate**: **37.04%** across all bookings.
2. **Hotel Type Matters**: City Hotel has a significantly higher cancellation rate (**41.73%**) compared to Resort Hotel (**27.76%**).
3. **Lead Time Impact**: Canceled bookings have nearly 2x longer lead times (**144.8 days** vs. **80.0 days** for non-canceled bookings).
4. **Customer Segmentation**:
   - **Transient** customers cancel the most (**40.75%**).
   - **Group bookings** cancel the least (**10.23%**).
5. **Booking Channel Risk**:
   - **Direct** bookings exhibit the lowest cancellation risk (**15.34%**).
   - **Group / Agency** channels experience the highest cancellation rate (**61.06%**).
6. **Pricing Dynamics (ADR)**: City Hotel commands a higher Average Daily Rate (**€105.30**) than Resort Hotel (**€94.95**).
7. **Seasonality**: Peak booking demand occurs in **August**, **July**, and **May**; demand hits yearly lows in **January**, **December**, and **November**.
8. **Room Type Pricing**: Room type **H** commands the highest Average Daily Rate at **€188.22/night**, followed by **G** at **€175.00/night**.

---

## 🎯 Business Recommendations
- **Target Long-Lead-Time Bookings**: Implement targeted automated reminders, non-refundable discount tiers, or progressive deposit schedules for bookings made >90 days in advance.
- **Incentivize Direct Bookings**: Promote direct booking channels over third-party group/agency channels to reduce high-churn cancellation risks.
- **Seasonal Staffing & Inventory Optimization**: Scale staffing, dynamic pricing algorithms, and room availability to maximize revenue during peak summer months (May–August).

---

## 📁 Repository Structure
- `Python-only-notebook.ipynb`: Complete exploratory data analysis (EDA), data cleaning, and statistical breakdowns in Python.
- `SQL-only.ipynb`: SQL-based analytical queries executed on an in-memory SQLite database.
- `hotel_bookings.csv`: Kaggle Hotel Booking Demand dataset.
