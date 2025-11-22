# 🛠️ Banggood ETL Pipeline & Analytics Dashboard

This project is an end-to-end **ETL Pipeline** built using **Python**,
**BeautifulSoup**, **Selenium/Playwright**, **Pandas**, **SQL Server**,
and **Streamlit**.\
It extracts product listings from **Banggood.com**, cleans and
transforms the data, stores it in a SQL database, and visualizes
insights using an interactive dashboard.

🚀 **Live Streamlit Dashboard:**\
👉 **https://banggood-pipeline-mkbbxuq7zzrh42rkydntpc.streamlit.app/**

------------------------------------------------------------------------

## 📌 Project Overview

### **1️⃣ Extract**

-   Scraped product listings from **https://banggood.com/**
-   Used BeautifulSoup + Selenium/Playwright to load dynamic content
-   Stored raw scraped data in a **CSV file**

### **2️⃣ Transform (Clean Data)**

-   Removed unwanted characters (`US$`, commas, special symbols)
-   Converted numeric fields (Price, Rating, Reviews) into proper
    datatypes
-   Fixed missing values (NULL standardization)
-   Saved cleaned output into a **clean CSV file**

### **3️⃣ Load**

-   Created SQL Server database & table using Python + SQLAlchemy
-   Loaded the cleaned CSV into SQL Server using `pandas.to_sql()`

### **4️⃣ Data Retrieval**

-   Queried database to retrieve metrics such as:
    -   Price insights\
    -   Category-level summaries\
    -   Rating analysis\
    -   Top-reviewed products

### **5️⃣ Analytics Dashboard**

Built using **Streamlit**, includes: - Total product count\
- Average price per category\
- Rating vs Price correlation\
- Top reviewed products\
- Price distribution\
- Category summaries

📌 **Deployed on Streamlit Cloud**

👉 https://banggood-pipeline-mkbbxuq7zzrh42rkydntpc.streamlit.app/

------------------------------------------------------------------------

## 📁 Project Structure

    ├── extract.py
    ├── clean.py
    ├── database_loader.py
    ├── analysis.py
    ├── app.py
    ├── raw_data.csv
    ├── clean_data.csv
    ├── README.md

------------------------------------------------------------------------

## 🧰 Technologies Used

-   Python\
-   BeautifulSoup\
-   Selenium / Playwright\
-   Pandas\
-   SQLAlchemy\
-   PyODBC\
-   Matplotlib\
-   Streamlit\
-   SQL Server

------------------------------------------------------------------------

## ▶️ How to Run Locally

### 1. Install dependencies

    pip install -r requirements.txt

### 2. Run ETL pipeline

    python extract.py
    python clean.py
    python database_loader.py

### 3. Launch Streamlit app

    streamlit run app.py

------------------------------------------------------------------------

## 🌐 Live Demo

👉 **Streamlit App:**
https://banggood-pipeline-mkbbxuq7zzrh42rkydntpc.streamlit.app/
