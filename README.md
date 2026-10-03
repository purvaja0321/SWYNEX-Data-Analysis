# SWYNEX – Data Cleaning & Preparation

## Project Title

**E-Commerce Sales Analytics & Insights**

## Internship Task

**Task 1 – Data Cleaning & Preparation**

## Objective

The objective of this task is to clean and prepare an e-commerce retail dataset for further analysis and dashboard development.

## Dataset

This project uses the **Online Retail Dataset**, which contains transaction-level information including:

* Invoice Number
* Stock Code
* Product Description
* Quantity
* Invoice Date
* Unit Price
* Customer ID
* Country

## Data Quality Issues Identified

The raw dataset was checked for:

* Missing values
* Duplicate records
* Incorrect data types
* Inconsistent text values
* Invalid quantity values
* Invalid unit price values

## Cleaning Performed

The dataset was cleaned using **Python and Pandas**.

The following steps were performed:

1. Removed duplicate records.
2. Removed leading and trailing spaces from text columns.
3. Handled missing product descriptions.
4. Removed records with missing Customer IDs.
5. Removed records with Quantity less than or equal to zero.
6. Removed records with Unit Price less than or equal to zero.
7. Converted `InvoiceDate` to datetime format.
8. Converted `Quantity` and `CustomerID` to appropriate numeric data types.
9. Converted `UnitPrice` to numeric format.
10. Created a new `TotalAmount` column using:

```text
TotalAmount = Quantity × UnitPrice
```

## Dataset Results

### Before Cleaning

* Records: **541,909**
* Columns: **8**

### After Cleaning

* Records: **392,692**
* Columns: **9**

The additional column is `TotalAmount`, which will be useful for future sales and revenue analysis.

## Cleaned Dataset

Due to the large file size, the cleaned CSV is hosted separately on Google Drive.

**Cleaned Dataset:** https://drive.google.com/file/d/14ruQ2_E_tumlDvoeOT6q7pA4ox0fWbz_/view?usp=sharing

## Project Files

```text
SWYNEX-Data-Cleaning-Preparation/
│
├── main/
    └── Data_Cleaning_Preparation.ipynb
    │ 
    └── README.md
```

## Tools Used

* Python
* Pandas
* NumPy
* Jupyter Notebook
* Microsoft Excel

## Dataset Source

**Online Retail Dataset – UCI Machine Learning Repository**

## Outcome

The raw e-commerce transaction dataset was successfully cleaned and prepared for the next stages of the project, including:

* Exploratory Data Analysis
* Sales and Revenue Analysis
* Product Performance Analysis
* Customer Analysis
* Interactive Power BI Dashboard

