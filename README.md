# Optimizing Customer Value: RFM Based Segmentation in Online Retail
- cleaned data: https://drive.google.com/file/d/1dJulk0WURXMbOGvTUaP82_jh2Ns1z2ts/view?usp=share_link

- Tableau Public: https://public.tableau.com/views/CapstoneProject_17138013092280/OnlineRetailSales?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link
# Optimizing Customer Value: RFM Based Segmentation in Online Retail

This repository contains the LaTeX source code for the paper titled "Optimizing Customer Value: RFM Based Segmentation in Online Retail". The paper explores the use of RFM (Recency, Frequency, Monetary) analysis and K-means clustering to segment customers in the online retail sector and tailor marketing strategies accordingly.

## Introduction

In today's online retail world, understanding customer value is crucial for success. Businesses utilize various methods like surveys and market research to learn about customer needs and tailor their offerings and marketing strategies accordingly. This personalized approach not only boosts customer satisfaction but also drives growth in the competitive online retail market. These methods serve as invaluable tools, providing insights that guide strategic decision-making and enhance overall business performance.

## Problem Statement

This project aims to address the complexity arising from the overwhelming volume of customer data available in the digital realm. Businesses require sophisticated analytical methods to sift through this data and extract actionable insights. Thus, there is a need for tools that can navigate through this data maze and provide meaningful insights into customer behavior and preferences. This will be accomplished by leveraging data analytics methods, particularly RFM analysis, to gain a deeper understanding of customer value in online retail.

## Dataset Description

The dataset used in this project is a transnational dataset containing all the transactions that occurred between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company primarily sells unique and all-occasion gifts.

### Variables Description

- **InvoiceNo:** Invoice number, a six-digit integral number uniquely assigned to each transaction. If this code starts with the letter 'C', it indicates a cancellation.
- **StockCode:** Product code, a five-digit integral number uniquely assigned to each distinct product.
- **Description:** Product name.
- **Quantity:** The quantities of each product per transaction, numeric.
- **InvoiceDate:** Invoice Date and time, indicating the day and time when each transaction was generated.
- **UnitPrice:** Unit price, product price per unit in sterling, numeric.
- **CustomerID:** Customer number, a five-digit integral number uniquely assigned to each customer.
- **Country:** Country name, indicating the name of the country where each customer resides.

## Methodology

The project utilized a multi-step approach to analyze customer behavior and value in the online retail sector. 

### Data Cleaning and Wrangling

The initial phase of the project involved data cleaning to ensure the integrity and quality of the dataset. The dataset, sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx), underwent a meticulous cleaning process. This included checking for missing data and removing duplicate records to eliminate any inconsistencies.

Upon initial loading and inspection of the dataset, several challenges were identified, necessitating data wrangling to prepare it for analysis. Some of the key challenges encountered and the corresponding actions taken include:

- **Missing Values in 'Description' and 'CustomerID' Columns:** Attempted to link each InvoiceNo to a single CustomerID to fill missing values, but no linkage was found. As missing CustomerID values could not be filled, observations with NaN values in the CustomerID column were dropped. Dropping NaN values in the CustomerID column also removed all missing Description rows.
- **Transactions from the last month of 2011 only had data for 9 days:** they were also removed.

### Exploratory Data Analysis (EDA)

Following data cleaning, EDA was conducted to gain insights into the structure and distribution of the data. Various analyses were performed to understand the characteristics of the dataset and identify patterns and trends.

### Cohort Analysis

Cohort analysis is a powerful tool for understanding customer behavior over time, particularly in terms of retention and loyalty.

### Data Modeling

#### Recency, Frequency, Monetary (RFM) Analysis

RFM analysis is a method used to analyze customer behavior based on three key metrics: Recency, Frequency, and Monetary value.

#### K-means Clustering

K-means clustering was utilized to segment customers based on their RFM scores and other relevant features.

## Results

The data analysis phase of the project yielded valuable insights into various aspects of the online retail business.

## Conclusion

Understanding customer value is vital in today's online retail landscape. Traditional methods like surveys and market research provide valuable insights, but with the vast amount of customer data available, businesses must adopt sophisticated analytical methods to extract actionable insights.

## Future Scope

Moving forward, there are several avenues for future research and development in this area.

## Author

- **Deepti Gururaj Baragi** - April 23, 2024

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
