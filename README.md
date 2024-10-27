# 🚚 **B2B Shipping Cost Accuracy: Analysis and Prediction**

## 📋 **Problem Statement:**
- ABC Company is facing issues with discrepancies between their estimated shipping costs and the actual charges they receive from courier companies. These differences can lead to financial losses and unhappy customers.
- The company wants to make sure the shipping fees from couriers match their own cost estimates, which are based on factors like product weight and delivery zones.
- The goal is to build a solution that analyzes these differences and predicts future shipping costs more accurately, helping to spot overcharges or undercharges.

## 🎯 **Objective:**
- The main aim is to improve the accuracy of shipping cost predictions by:
  - **Analyzing** past shipment data to identify cost differences.
  - **Predicting** future shipping costs using machine learning models.
  - **Highlighting** where the actual charges from couriers don’t match the company’s estimates.
  - **Improving** the company's financial and operational efficiency by reducing billing errors.

## 📊 **Dataset Overview:**
ABC Company is using several datasets to solve this problem:

### 1️⃣ **Courier Rates Data**
- Information on shipment charges:
  - **Forward Charges**: The rates for sending products to customers in different zones (A, B, C, D, E).
  - **Return Charges**: Rates for sending products back to the origin (return shipments) for the same zones.

### 2️⃣ **Invoice Data**
- Contains shipment details:
  - **AWB Code** & **Order ID**: Unique shipment identifiers.
  - **Charged Weight**: The weight on which the courier calculated the charge.
  - **Warehouse Pincode** & **Customer Pincode**: Locations for pickup and delivery.
  - **Zone**: The delivery area based on pincodes.
  - **Type of Shipment** & **Billing Amount (Rs.)**: The shipment type and the amount billed for it.

### 3️⃣ **Order Report**
- Details about the items in the order:
  - **ExternOrderNo**: Reference number for the order.
  - **SKU**: Product code.
  - **Order Qty**: Number of items ordered.

### 4️⃣ **Pincode Data**
- Pincodes linked to delivery zones:
  - **Warehouse Pincode** & **Customer Pincode**: Shows how pincodes map to different delivery zones.

### 5️⃣ **SKU Master Data**
- Product information:
  - **SKU**: Product identifier.
  - **Weight (g)**: Weight of each product in grams.

## 🛠️ **Project Workflow:**
- **Data Cleaning**: Prepare the data by fixing errors, filling missing values, and formatting it for analysis.
- **Predictive Modeling**: Build a machine learning model that predicts shipping costs based on historical data. This includes selecting key features, training the model, and testing its accuracy.
- **Discrepancy Analysis**: Compare the predicted shipping costs with actual courier charges to find any differences.
- **Visualization**: Use charts and tables to show the model’s predictions, accuracy, and any significant discrepancies.

## 📈 **Final Output Table:**
The project will produce a table that compares ABC’s cost estimates with the actual courier charges. It will include:

- **Order ID**: The unique identifier for each order.
- **Total Weight**: The total weight of the order.
- **Weight Slab**: The weight category the order falls under.
- **Delivery Zone as per ABC**: The zone according to ABC's system.
- **Expected Charge as per ABC (Rs.)**: What ABC expects to be charged.
- **AWB Number**: Tracking number.
- **Total Weight as per Courier Company (KG)**: The weight used by the courier to calculate the charge.
- **Delivery Zone Charged by Courier Company**: The zone charged by the courier.
- **Billing Amount (Rs.)**: The amount billed by the courier.
- **Weight Slab Charged by Courier Company (KG)**: The weight category used by the courier for billing.

### Example:

| Order ID   | Total Weight | Weight Slab | Delivery Zone as per ABC | Expected Charge (Rs.) | AWB Number | Total Weight (KG) | Courier Zone | Billing Amount (Rs.) | Courier Weight Slab (KG) |
|------------|--------------|-------------|---------------------------|-----------------------|------------|-------------------|--------------|----------------------|--------------------------|
| 2001827036 | ...          | ...         | ...                       | ...                   | ...        | ...               | ...          | ...                  | ...                      |
| 2001821995 | ...          | ...         | ...                       | ...                   | ...        | ...               | ...          | ...                  | ...                      |
| ...        | ...          | ...         | ...                       | ...                   | ...        | ...               | ...          | ...                  | ...                      |

## 📊 **Summary Table:**
A summary table will provide an overall view of the shipping cost discrepancies:

- **Total Orders with Correct Charges**
- **Total Orders Overcharged**
- **Total Orders Undercharged**

### Example:

| Description                              | Count | Amount (Rs.) |
|------------------------------------------|-------|--------------|
| Correct Charges                          | ...   | ...          |
| Overcharged Orders                       | ...   | ...          |
| Undercharged Orders                      | ...   | ...          |

## ✅ **Conclusion:**
- This project focuses on making sure shipping charges are accurate for ABC Company.
- By analyzing past data and building a predictive model, the company can spot billing errors and forecast shipping costs more accurately.
- Reducing shipping cost errors will help ABC save money, improve efficiency, and avoid disputes with courier partners.

### **Relevance to Logistics and Supply Chain:**
- Accurate shipping cost predictions are crucial for financial planning and maintaining good relationships with courier partners.
- This project will help ABC Company improve its budgeting and cost control, leading to smoother operations and higher customer satisfaction.
