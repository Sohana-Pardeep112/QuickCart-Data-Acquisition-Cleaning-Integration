# QuickCart – Data Acquisition, Cleaning & Integration

## Project Overview

**QuickCart Pakistan** is a fictional e-commerce business used as a case study for a Business Analytics assignment.

The project focuses on collecting, inspecting, cleaning, preprocessing, and integrating business data to prepare it for reliable analysis.

The business scenario involves declining product ratings and increasing product returns. The objective is to demonstrate how data analysts can identify data-quality issues, combine information from different sources, and prepare meaningful data for business decision-making.

## Objectives

- Understand and explore raw business datasets.
- Identify data-quality issues before performing analysis.
- Clean missing, duplicate, inconsistent, and invalid records.
- Integrate order data with product information.
- Create meaningful analytical features.
- Explore relationships between product categories, ratings, returns, and delivery performance.
- Practice web scraping and API-based data acquisition.

## Technologies & Tools

| Technology | Purpose |
|---|---|
| Python | Data processing and analysis |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Jupyter Notebook | Analysis and documentation |
| Requests | HTTP requests and data acquisition |
| BeautifulSoup | HTML parsing and web scraping |
| REST API | Retrieving external JSON data |
| JSON | Handling structured API responses |

## Project Workflow

### 1. Data Loading & Exploration
- Importing datasets using Pandas.
- Examining dataset dimensions, columns, and data types.
- Identifying numerical, categorical, date/time, identifier, and textual variables.

### 2. Data Quality Audit
Investigating:
- Missing values
- Duplicate records
- Inconsistent category labels
- Invalid and suspicious numerical values
- Date inconsistencies
- Potential outliers
- Unmatched product identifiers

### 3. Data Cleaning & Preprocessing
Applying appropriate cleaning techniques based on the business context:
- Handling missing values.
- Removing or resolving duplicate records.
- Standardizing text and category labels.
- Correcting invalid values where justified.
- Converting columns into appropriate data types.
- Parsing and validating dates.
- Investigating outliers instead of automatically deleting them.

### 4. Data Integration
- Integrating cleaned order data with the product master dataset.
- Selecting an appropriate join method.
- Checking unmatched Product_ID values.
- Validating the merged dataset to prevent accidental duplication.

### 5. Feature Engineering & Business Analysis

Creating at least four useful business features, such as:
- Delivery_Days
- Net_Unit_Price
- Order_Value
- Late_Delivery
- Rating_Band
- High_Discount

Investigating business questions:
- Which product categories generate the highest total order value?
- Do returned orders have different average ratings?
- Which cities have the longest average delivery times?
- Are late deliveries associated with lower customer ratings?
- What additional patterns should management investigate?

### 6. Web Scraping
Using the Books to Scrape practice website to:
- Send HTTP requests using Requests.
- Parse HTML using BeautifulSoup.
- Extract at least 20 book titles, prices, and ratings.
- Store the extracted information in a Pandas DataFrame.
- Export the data as a CSV file.

### 7. API & JSON Data Acquisition
Using the JSONPlaceholder public testing API to:
- Send GET requests.
- Verify HTTP response status.
- Retrieve user records in JSON format.
- Convert API responses into a Pandas DataFrame.
- Export the resulting dataset as CSV.

## Dataset Information

The assignment provides two primary datasets:

| Dataset | Description |
|---|---|
| `quickcart_raw.csv` | Raw order and customer data containing intentional data-quality issues |
| `quickcart_products.csv` | Product master data used for data integration |

Additional datasets are collected through web scraping and API requests.

## Expected Deliverables

- Completed Jupyter Notebook.
- Cleaned and integrated QuickCart dataset.
- Scraped book dataset.
- API user dataset.
- Data quality audit and cleaning explanations.
- Feature engineering and business analysis.
- Executive summary for management.

## Key Learning Outcomes

Through this project, I developed practical understanding of:

- Business data collection and acquisition.
- Data quality assessment and preprocessing.
- Data cleaning and transformation.
- Data integration and merging.
- Feature engineering.
- Exploratory data analysis.
- Web scraping.
- REST API integration and JSON handling.
- Translating data-quality findings into business recommendations.

## Repository Structure

```text
QuickCart-Data-Analytics/
│
├── data/
│   ├── quickcart_raw.csv
│   └── quickcart_products.csv
│
├── notebooks/
│   └── BA3002_A1_RollNo.ipynb
│
├── outputs/
│   ├── quickcart_clean_RollNo.csv
│   ├── scraped_books_RollNo.csv
│   └── api_users_RollNo.csv
│
└── README.md
```

*Note: The folder structure above is a suggested organization for the final GitHub repository.*

## Project Information

**Course:** BA3002 – Business Data and Text Mining  
**Project:** Assignment 01  
**Case Study:** QuickCart Pakistan  
**Program:** BS Business Analytics  

---

*This project demonstrates the importance of preparing trustworthy, explainable, and analysis-ready data before applying advanced analytical techniques.*
