# **Food Delivery Cost and Profitability Analysis**  

## **Project Overview**  
This project aims to analyze the **costs, revenues, and profitability** of a food delivery service. By examining **order values, commission fees, delivery times, and refund trends**, we derive key insights to optimize operations and enhance profitability.  

The analysis covers aspects such as:  
✅ Identifying the **most common payment method and its proportion**  
✅ Calculating the **average order value and commission fees**  
✅ Analyzing **delivery times and customer payment behavior**  
✅ Evaluating **refund trends and chargebacks**  
✅ Conducting **statistical hypothesis testing** on delivery efficiency  
 
 ---
 
## **Table of Contents**  
- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Project Structure](#project-structure)  
- [Key Findings](#key-findings)  
- [Technologies Used](#technologies-used)  
- [Setup & Execution](#setup--execution)  
- [Business Recommendations](#business-recommendations)  
- [Author](#author)  

---

## **Dataset**  
📂 The dataset contains **1,000 orders** with the following attributes:  

| Column Name               | Description |
|---------------------------|-------------|
| **Order ID**              | Unique identifier for each order |
| **Customer ID**           | Unique customer identifier |
| **Restaurant ID**         | Unique restaurant identifier |
| **Order Date and Time**   | Timestamp when the order was placed |
| **Delivery Date and Time** | Timestamp when the order was delivered |
| **Order Value**           | Total value of the order (₹) |
| **Delivery Fee**          | Fee charged for order delivery (₹) |
| **Payment Method**        | Payment type used (Credit Card, Digital Wallet, Cash on Delivery) |
| **Discounts and Offers**  | Discounts applied to the order (if any) |
| **Commission Fee**        | Fee charged by the platform per order (₹) |
| **Payment Processing Fee** | Transaction processing fee (₹) |
| **Refunds/Chargebacks**   | Refund amount if the order was disputed (₹) |

---

## **Project Structure**  

📁 **Project Folder**  
```
/food_delivery_analysis  
│── data/  
│   ├── food_orders_new_delhi.csv  
│── notebooks/  
│   ├── food_delivery_analysis.ipynb  
│── src/  
│   ├── data_cleaning.py  
│   ├── data_analysis.py  
│── README.md  
│── requirements.txt  
│── results/  
│   ├── charts/  
│   ├── summary_report.pdf  
```

- **data/** → Contains the dataset (`food_orders_new_delhi.csv`).  
- **notebooks/** → Jupyter notebook with exploratory data analysis (EDA).  
- **src/** → Python scripts for **data cleaning and analysis**.  
- **results/** → Stores **charts, reports, and summary insights**.  
- **requirements.txt** → Lists required Python libraries.  

---

## **Key Findings**  

### 🔹 **1. Payment Method Trends**  
✅ The **most common payment method** accounts for **32.73% to 38.67%** of transactions.  
✅ Cash on Delivery orders **tend to have higher order values** than Digital Wallet payments.  

### 🔹 **2. Revenue Insights**  
✅ The **average commission fee per order** is **₹126.99**, with a **median of ₹127.00**.  
✅ Customers spend **₹1053.97 per order on average**.  
✅ **55% of orders contribute a commission fee greater than ₹120**, impacting revenue positively.  

### 🔹 **3. Delivery Time Analysis**  
✅ The **average delivery time** for **Credit Card orders is 74.01 minutes**, which is relatively high.  
✅ **50% of deliveries take between 50 to 96 minutes**.  
✅ **Hypothesis testing** confirmed that **delivery time is significantly greater than 53 minutes**, indicating potential inefficiencies.  

### 🔹 **4. Refund and Chargeback Trends**  
✅ **Credit Card transactions** have the highest refund cases (**102 cases**), followed by **Cash on Delivery (101 cases)** and **Digital Wallet (82 cases)**.  
✅ This suggests a need for **better payment dispute resolution strategies**.  

---

## **Technologies Used**  

🔹 **Programming Language**: Python 🐍  
🔹 **Libraries & Frameworks**:  
- `pandas` → Data processing  
- `numpy` → Numerical computations  
- `matplotlib` & `seaborn` → Data visualization  
- `scipy.stats` → Statistical analysis  

---

## **Setup & Execution**  

### **1️⃣ Install Dependencies**  
Ensure you have **Python 3.x** installed. Run the following command to install the required libraries:  

```bash
pip install -r requirements.txt
```

### **2️⃣ Run the Jupyter Notebook (Recommended)**  
To explore the dataset and analysis in an interactive way:  

```bash
jupyter notebook notebooks/food_delivery_analysis.ipynb
```

### **3️⃣ Run the Python Scripts**  
Alternatively, you can execute the analysis scripts from the command line:  

```bash
python src/data_cleaning.py  
python src/data_analysis.py  
```

---

## **Business Recommendations**  

### **1️⃣ Optimize Delivery Efficiency**  
- **Reduce delivery times** by improving **logistics operations**.  
- Implement **real-time tracking and predictive ETA models**.  

### **2️⃣ Encourage Digital Payments**  
- Offer **cashback or discounts** for Digital Wallet users to increase their average spending.  

### **3️⃣ Manage Refunds & Chargebacks**  
- **Credit Card transactions** have the highest refunds; implement **fraud detection measures**.  
- Educate customers on **payment security** to increase trust in Digital Wallets.  

### **4️⃣ Increase Order Value & Revenue**  
- Introduce **bundle offers or premium services** to increase per-order spending.  
- Implement **AI-driven recommendations** to suggest add-ons and increase basket size.  
