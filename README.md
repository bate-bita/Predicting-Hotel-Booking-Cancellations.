# Hotel Cancellations Analytics  

This project explores how machine learning can help hotels predict booking cancellations and make smarter operational decisions. Using real data from two Portuguese hotels, the analysis identifies key factors that influence cancellations and compares multiple models to find the most reliable predictive solution.  

📄 [View Project Presentation (PDF)](./Hotel%20Booking%20Cancellations%20Presentation.pdf?raw=true)

---

## Project Overview  

Hotel bookings often face uncertainty due to last-minute cancellations, affecting revenue, staffing, and resource planning.  
This project applies a data-driven approach to forecast cancellations, helping hotel managers anticipate demand and reduce overbooking risks.  

**Goal:** Predict whether a booking will be cancelled based on guest and reservation characteristics.  
**Duration Covered:** July 2015 – August 2017  
**Dataset Size:** 119,390 observations, 31 features  

---

## Dataset Summary  

- Source: Research data published by Nuno Antonio, Ana de Almeida, and Luis Nunes (Elsevier Inc.)  
- Type: Real hotel management system (PMS) data from City and Resort Hotels in Portugal  
- Features include: lead time, market segment, customer type, deposit type, and prior cancellation history  

---

## Approach  

**1. Data Preparation**  
- Cleaned and merged datasets from two hotels  
- Handled missing values and removed redundant features (e.g., ReservationStatus and Country) to avoid bias  
- Split data into training and testing sets for model validation  

**2. Exploratory Data Analysis (EDA)**  
- Visualised booking patterns across customer type, deposit type, and market segment  
- Highlighted imbalance in the target variable (`IsCanceled`) showing fewer cancellations than confirmed bookings  

**3. Feature Engineering**  
- Examined correlations between variables and cancellation likelihood  
- Identified the top five influential features:  
  *Lead time, Previous Cancellations, Booking Changes, Parking Requests, Special Requests*  

**4. Model Development & Evaluation**  
- Trained and tuned four classifiers: **Logistic Regression, K-Nearest Neighbours, Decision Tree, Random Forest**  
- Optimised hyperparameters using GridSearchCV  
- Evaluated performance using **Precision, Recall, and F1 Score** due to class imbalance  

---

## Key Findings  

| Model | Precision | Recall | F1 Score |  
|:------|:-----------|:--------|:----------|  
| Logistic Regression | 82.6% | 64.6% | 72.5% |  
| Decision Tree | 78.2% | **78.0%** | 75.9% |  
| KNN | 76.5% | 73.7% | 77.3% |  
| Random Forest | **87.3%** | 77.3% | **82.0%** |  

- **Decision Tree** achieved the highest recall (78%), effectively capturing most cancellations.  
- **Random Forest** achieved the best overall balance with an F1 score of **82%**, offering strong precision and recall.  
- Insights suggest that early bookings and repeat customers behave differently, enabling targeted policy adjustments.  

---

## Tools and Techniques  

- **Languages & Libraries:** Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Skills Demonstrated:** Data wrangling, EDA, feature selection, model evaluation, report automation  
- **Metrics Used:** Precision, Recall, F1-Score, Confusion Matrix  
- **Ethical Consideration:** Excluded sensitive features (e.g., Country) to avoid potential geographic bias in model predictions  

---

## Outcome  

This project demonstrates how predictive analytics can support operational planning and revenue management in the hospitality industry.  
It highlights an analytical process from raw data cleaning to business insight communication, showing strong capabilities in:  

- Analytical storytelling  
- Performance reporting  
- Translating technical models into business impact  

---

## Author  

👩🏽‍💻 **Bate Bita Tambe**  
Business and Data Analyst  
[LinkedIn](https://www.linkedin.com/in/bate-bita-tambe-a29ab6221)
