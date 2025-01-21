# SEC Financial Statement Data Analysis

This project involves analyzing financial statement data obtained from the U.S. Securities and Exchange Commission (SEC) for the first four months of 2024. The dataset includes various tables such as `SUB`, `TAG`, `DIM`, `REN`, `PRE`, `NUM`, `TXT`, and `CAL`, which contain information about submissions, tags, dimensions, rendering, presentation, numeric data, text data, and calculations, respectively.

## Dataset Source
The dataset was officially obtained from the SEC website. You can find more details and download the dataset from the following link:
[SEC Financial Statement Data Sets](https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets)

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

### 3. **Data Analysis**
   - **Question 1:** Retrieved the submission ID, company name, submission date, and full mailing address for all submissions made by companies in the “Healthcare” sector in March 2024.
     - **Insight:** Identified 20 companies in the healthcare sector that submitted financial statements in March 2024. The companies include INVACARE HOLDINGS CORP, U S PHYSICAL THERAPY INC, and BIODESIX INC, among others.

   - **Question 2:** Calculated and displayed the month, the total number of submissions, and the average number of submissions for the first four months of 2024.
     - **Insight:** The total number of submissions varied each month, with January having 5,904 submissions, February having 9,400, March having 9,032, and April having 9,634. The average number of submissions across these months was 8,492.5.

   - **Question 3:** Retrieved the list of all tag IDs, tag names, and the total number of companies that used each tag for all tags used in submissions by companies in the “Finance” sector in 2024.
     - **Insight:** The most commonly used tags in the finance sector include "Assets," "Entity Common Stock, Shares Outstanding," and "Liabilities," with 1,476, 1,456, and 1,443 companies using these tags, respectively.

   - **Question 4:** Retrieved the top 5 companies with the highest total assets in 2024, including their company name, sector, and the number of unique tags used in their submissions.
     - **Insight:** The top company by total assets is BANK OF CHILE, with total assets amounting to 16,048,901,542,880,200,602.86. Other top companies include POSCO HOLDINGS INC., BANCO SANTANDER CHILE, KB FINANCIAL GROUP INC., and SHINHAN FINANCIAL GROUP CO LTD.

## Repository Structure
- **Notebooks:** Contains the Jupyter notebook (`Final_Asgn2_G6.ipynb`) with the complete code and analysis.
- **Data:** Includes the raw data files downloaded from the SEC website and the processed `.csv` files.
- **README.md:** This file, providing an overview of the project and its findings.

## How to Run the Project
1. **Clone the Repository**
2. **Set Up the Environment**
3. **Run the Jupyter Notebook**

## Conclusion
This project provides a comprehensive analysis of financial statement data from the SEC, focusing on specific sectors and financial metrics. The insights gained from this analysis can be valuable for understanding trends and patterns in financial reporting.

For any questions or further information, please feel free to reach out.

---

**Note:** Ensure that you have the necessary permissions and access to the SEC dataset before using it for analysis.
