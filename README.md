# Yelp Data Pipeline 📊🛠️

This project demonstrates a scalable data pipeline that transforms and structures over 6 million Yelp reviews.  
It extracts data from JSON files, processes them into analysis-ready DataFrames using **Python**, and stores them into a relational database.  
The final data is suitable for BI tools such as **Tableau** or **Power BI** for downstream visualization and insights.

---

## 🗂️ Datasets Used

- `business.json` — business metadata (location, category, stars)
- `review.json` — user reviews for businesses
- `user.json` — reviewer profile and review counts
- `tip.json` — tips given by users
- `checkin.json` — check-in data by time

> Source: [Yelp Open Dataset](https://www.yelp.com/dataset)

---

## 🧰 Tools & Technologies

- **Python**: Data handling (Pandas, JSON), scripting
- **Jupyter Notebook**: EDA and pipeline prototyping
- **SQLite**: For local relational data storage
- **SQLAlchemy**: For database operations (can be scaled to Azure SQL)
- **Tableau** (optional): For building dashboards

---

## ⚙️ Pipeline Steps Overview

1. **Load JSON files**  
   Use Python's `json` and `pandas` to parse Yelp dataset files

2. **Clean & Normalize Data**  
   Convert nested structures, drop unnecessary fields, fix data types

3. **Create SQL Table Schemas**  
   Define table structures based on normalized dataframes

4. **Insert into SQLite Database**  
   Use `SQLAlchemy` to write clean tables into a `.db` file

5. *(Optional)* Connect Tableau to SQLite/Azure SQL for BI visualization

---

## 📁 Project Structure
yelp-data-pipeline/ ├── yelp_data.ipynb 
Yelp JSON files (Kaggle) ├── yelp_database.db 

---

## 🚀 How to Run

1. Clone the repo:

    ```bash
    git clone https://github.com/a0828451/yelp-data-pipeline.git
    cd yelp-data-pipeline
    ```

2. Install Python dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Run the notebook:

    ```bash
    jupyter notebook yelp_data.ipynb
    ```

4. (Optional) Connect Tableau to `yelp_database.db` or Azure SQL for analysis

---

## 📊 Sample Use Cases

- Discover most reviewed restaurants in Las Vegas
- Analyze reviewer behavior (e.g., number of reviews vs. stars)
- Identify business categories with highest engagement
- Build interactive dashboards in Tableau

---

## 👤 Author

**Yun-Shan Chung**  
[GitHub](https://github.com/a0828451) | Data Pipeline · SQL · Visualization

> Feel free to fork this repo or reach out if you're working with Yelp data too!



