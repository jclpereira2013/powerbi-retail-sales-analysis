![Dashboard Overview](images/overview.png)

# 📊 Power BI Superstore Dashboard

## 🧠 Project Overview

This project presents an end-to-end data analysis solution using Power BI, focused on retail sales performance, customer behavior, and logistics efficiency.

The solution includes:

* Data cleaning and transformation (Power Query)
* Star schema data model
* Advanced DAX measures
* Interactive dashboard for business insights

---

## 📁 Dataset

* Source: Superstore Retail Dataset
* Records: Orders at transactional level
* Main fields: Sales, Profit, Discount, Customer, Region, Shipping

---

## 🏗️ Data Model

A star schema was implemented with the following structure:

### Fact Table

* FactPedidos

  * Order ID
  * Order Date
  * Ship Date
  * Sales
  * Profit
  * Discount
  * Quantity
  * Shipping Cost

### Dimensions

* DimCliente
* DimProducto
* DimFecha
* DimEnvio

---

## 📐 Key Metrics (DAX)

### Sales & Profit

* Total Sales
* Total Profit
* Profit Margin %

### Customer Analysis

* Total Customers

### Logistics

* Avg Ship Days
* On-Time Delivery %
* Shipping Cost per Order

---

## 📊 Dashboard Pages

### 1. Overview

High-level KPIs and sales trends

### 2. Profit Deep Dive

Analysis by category, segment, and discount impact

### 3. Client Analysis

Customer segmentation and purchase behavior

### 4. Logistics & Operations

Shipping performance and cost analysis

---

## 🖼️ Dashboard Preview

![Overview](images/overview.png)
![Sales](images/profitdeepdive.png)
![Customers](images/clientanalysis.png)
![Logistics](images/logistics&operations.png)

---

## 🚀 Key Insights

* High discounts negatively impact profit margins
* A small group of customers drives a large portion of sales
* Shipping mode significantly affects delivery time and cost
* Certain regions show operational inefficiencies

---

## 🛠️ Tools Used

* Power BI
* DAX
* Power Query

---

## 👤 Author

Juan Carlos Lopez Pereira

