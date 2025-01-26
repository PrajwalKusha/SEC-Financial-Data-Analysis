# SEC Financial Statement Data Analysis

This project involves analyzing financial statement data obtained from the U.S. Securities and Exchange Commission (SEC) for the first four months of 2024. The dataset includes various tables such as `SUB`, `TAG`, `DIM`, `REN`, `PRE`, `NUM`, `TXT`, and `CAL`, which contain information about submissions, tags, dimensions, rendering, presentation, numeric data, text data, and calculations, respectively.

## Dataset Source
The dataset was officially obtained from the SEC website. You can find more details and download the dataset from the following link:
[SEC Financial Statement Data Sets](https://www.sec.gov/data-research/sec-markets-data/financial-statement-notes-data-sets)

## Technologies Used
- **AWS (Amazon Web Services):** The project was hosted on AWS, providing a scalable and reliable cloud infrastructure.
- **EC2 Instance:** An Amazon EC2 instance was used to run the Jupyter Notebook and PostgreSQL database, ensuring efficient data processing and analysis.
- **Jupyter Notebook:** The primary tool for writing and executing the code, enabling interactive data analysis and visualization.
- **SQL:** Structured Query Language (SQL) was used extensively to query and manipulate the data stored in the PostgreSQL database.
- **Programming Language:** Bash was the main programming language used for data processing, analysis, and automation.
- **Ubuntu:** The operating system used on the EC2 instance, providing a stable and secure environment for running the project.
- **PostgreSQL:** A powerful open-source relational database system used to store and manage the financial data.

## Project Overview
The project is divided into several steps, including setting up the database, loading the data, and performing data analysis. The analysis focuses on answering specific questions related to the financial data, such as identifying companies in specific sectors, calculating submission statistics, and retrieving top companies based on financial metrics.

## Key Steps and Insights

### 1. **Setting Up the Database**
   - Installed necessary libraries (`ipython-sql`, `psycopg2`) to connect to PostgreSQL.
   - Created and connected to the `DMA_G6` database.
   - Defined and created tables (`SUB`, `TAG`, `DIM`, `REN`, `PRE`, `NUM`, `TXT`, `CAL`) with appropriate schemas and comments.

### 2. **Loading Data**
   - Downloaded and unzipped the dataset files for the first four months of 2024.
   - Converted `.tsv` files to `.csv` format for easier processing.
   - Stacked the data from all four months into single files for each entity.
   - Loaded the data into the respective tables in the PostgreSQL database.

### 3. **Data Analysis - Key Takeaways and Conclusions**

1. **Healthcare Sector Analysis (Analysis 1):**
   - **Key Takeaway:** Companies in the healthcare sector, such as INVACARE HOLDINGS CORP, U S PHYSICAL THERAPY INC, and BIODESIX INC, actively submitted financial statements in March 2024. This highlights the sector's compliance with SEC reporting requirements and provides insights into the financial health of these companies.
   - **Conclusion:** The healthcare sector remains a significant contributor to financial filings, with consistent submissions reflecting the industry's regulatory adherence and transparency.

2. **Submission Trends (Analysis 2):**
   - **Key Takeaway:** The number of submissions fluctuated monthly, with January (5,904), February (9,400), March (9,032), and April (9,634) showing varying levels of activity. The average number of submissions across these months was 8,492.5.
   - **Conclusion:** The data indicates a peak in submissions during February, possibly due to end-of-year financial reporting deadlines. Understanding these trends can help predict future submission volumes and optimize resource allocation for data processing.

3. **Finance Sector Tag Usage (Analysis 3):**
   - **Key Takeaway:** The most frequently used tags in the finance sector are "Assets," "Entity Common Stock, Shares Outstanding," and "Liabilities," with 1,476, 1,456, and 1,443 companies using these tags, respectively.
   - **Conclusion:** These tags are critical for financial reporting in the finance sector, reflecting the importance of asset management, equity tracking, and liability reporting. Companies in this sector prioritize these metrics to maintain compliance and transparency.

4. **Top Companies by Total Assets (Analysis 4):**
   - **Key Takeaway:** BANK OF CHILE leads with the highest total assets (16,048,901,542,880,200,602.86), followed by POSCO HOLDINGS INC., BANCO SANTANDER CHILE, KB FINANCIAL GROUP INC., and SHINHAN FINANCIAL GROUP CO LTD. These companies also utilize a high number of unique tags in their submissions.
   - **Conclusion:** The dominance of financial institutions in the top assets list underscores the sector's significant economic impact. The use of diverse tags indicates comprehensive financial reporting practices, which are essential for stakeholders and regulatory bodies.

### Overall Conclusion:
This analysis provides valuable insights into financial reporting trends across key sectors, such as healthcare and finance. The findings highlight the importance of regulatory compliance, the prevalence of specific financial metrics, and the economic significance of top-performing companies. These insights can guide stakeholders in making informed decisions and understanding sector-specific financial behaviors.

## Repository Structure
- **Notebooks:** Contains the Jupyter notebook with the complete code and analysis.
- **Data:** The dataset can be downloaded directly from the SEC Website. 
- **README.md:** This file, providing an overview of the project and its findings.

## How to Run the Project
1. **Clone the Repository**
2. **Set Up the Environment**
3. **Run the Jupyter Notebook**

## Conclusion
This project provides a comprehensive analysis of financial statement data from the SEC, focusing on specific sectors and financial metrics. The insights gained from this analysis can be valuable for understanding trends and patterns in financial reporting.

For any questions or further information, please feel free to reach out.
