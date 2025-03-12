# 📊 Equity Market Analysis Dashboard

An **interactive Power BI dashboard** for **historical stock price analysis**, enabling users to compare the performance of multiple companies and make **data-driven investment decisions**.

## 🚀 Features

✅ **Historical Stock Data Visualization** – Displays key financial trends over time.  
✅ **Key Financial Metrics** – Includes **P/E Ratio, EPS, ROE, ROIC, Price-to-Book, Free Cash Flow, and Earnings Yield**.  
✅ **Company Overview & Profile** – Displays industry, sector, CEO, and stock exchange details.  
✅ **Buy Consensus Analysis** – Shows market sentiment using Strong Buy, Buy, Hold, Sell, and Strong Sell indicators.  
✅ **SQL & Excel Integration** – Automates data extraction, transformation, and visualization.  
✅ **Performance Improvement** – Boosts market research efficiency by **40%** through automation.  

---

## 2️⃣ Database Setup

Ensure you have SQL Server/MySQL installed. Import the dataset using:


CREATE DATABASE StockMarketDB;
USE StockMarketDB;

CREATE TABLE stock_prices (
    id INT AUTO_INCREMENT PRIMARY KEY,
    company VARCHAR(255),
    date DATE,
    open_price FLOAT,
    close_price FLOAT,
    high_price FLOAT,
    low_price FLOAT,
    volume INT
);

LOAD DATA INFILE 'stock_data.csv'
INTO TABLE stock_prices
FIELDS TERMINATED BY ','
LINES TERMINATED BY '\n'
IGNORE 1 ROWS;






## 🖥️ Project Screenshots

### **Overview Page**
![Overview Screenshot](![Screenshot 2025-03-12 164953](https://github.com/user-attachments/assets/6d23b65c-d94f-4644-8f85-569a46d35820)
)

### **Company Profile**
![Profile Screenshot](![Screenshot 2025-03-12 165006](https://github.com/user-attachments/assets/f1553286-5a91-45a8-aad1-2d81b27ece31)
)

### **Historical Performance**
![Historical Performance Screenshot](![Screenshot 2025-03-12 165015](https://github.com/user-attachments/assets/88247e42-1e5c-4168-8fe1-f7f537861461)
)

---
## 3️⃣ Power BI Integration

1. Open Power BI and go to Home → Get Data → SQL Server.
2. Enter Server Details (use localhost for local SQL database).
3. Select StockMarketDB → Tables → Load Data.
4. Build visuals using Power BI charts, slicers, and DAX measures.

## 📌 Key Metrics Used

✅ P/E Ratio (Price-to-Earnings) – Indicates stock valuation.
✅ EPS (Earnings Per Share) – Measures company profitability.
✅ ROE (Return on Equity) – Evaluates financial performance.
✅ Debt-to-Equity Ratio – Assesses financial risk.
✅ Free Cash Flow (FCF) – Determines cash availability.
✅ Moving Averages – Identifies stock trends.

## 🔥 Advanced Features

🔹 DAX Measures for Custom Insights
🔹 🔄 Live Stock Market API Integration
🔹 📡 Real-time Data Refresh
🔹 📉 Predictive Analytics for Stock Trends
🔹 📌 AI-driven Sentiment Analysis (Future Scope)

## 🚀 Future Enhancements

🛠 API Integration for Live Stock Data
📉 AI-Powered Stock Price Prediction Model
📊 Enhanced User Interactivity with Drill-through Reports


## 🏆 Conclusion

This Equity Market Analysis Dashboard enables investors to make informed decisions using historical data trends and key financial metrics. 📊📈
