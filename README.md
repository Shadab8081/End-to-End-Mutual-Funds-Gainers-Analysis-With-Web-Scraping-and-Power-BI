# End-to-End-Mutual-Funds-Gainers-Analysis-With-Web-Scraping-and-Power-BI
## Project Objective:
- To extract, clean, and analyze mutual fund data from Yahoo Finance’s top gainers list and develop insightful KPIs and visualizations using Power BI, helping users understand mutual fund trends, performance, and key metrics.
# STEP:
## Web Scraping Mutual Fund Data from Yahoo Finance
# Objective :
- To extract mutual fund gainer data from Yahoo Finance using Python.
- Tool Used:
- requests: To send HTTP requests and retrieve web pages.
- BeautifulSoup: To parse HTML and extract table data.
- pandas: To store and process scraped data.
- time.sleep(): To add delay between requests (politeness to server).
# Data Cleaning and Transformation in Pandas
- Goals:Remove duplicates.
- Clean price and return columns.
- Replace -- with NaN, then fill missing values.
- Convert string percentages to float.
- Rename columns for clarity
## Key Questions / KPIs Answered:
- What is the average price of mutual funds currently?
- How are daily percentage changes distributed across funds?
- Which funds have the highest 3-month and YTD returns?
- What percentage of funds show positive year-to-date returns?
- What are the most volatile funds in terms of daily changes?
## DataUsed
- [yahoo_mutual_fund_gainers](https://github.com/Shadab8081/End-to-End-Mutual-Funds-Gainers-Analysis-With-Web-Scraping-and-Power-BI/blob/main/yahoo_mutual_fund_gainers.csv)
- [cleaned_mutual_fund_data](https://github.com/Shadab8081/End-to-End-Mutual-Funds-Gainers-Analysis-With-Web-Scraping-and-Power-BI/blob/main/cleaned_mutual_fund_data.csv)
## Process Overview:
- Data Collection:	Web scraping mutual fund gainers from Yahoo Finance using Python and BeautifulSoup
- Data Cleaning:	Removed nulls, standardized column names, converted percentages to numeric, and cleaned strings
- KPI Definition:	Created DAX measures for average price, return %, daily change %, etc.
- Visualization:	Built Power BI visuals including line charts, bar charts, and KPI cards
- Insights:	Interpreted visual data to provide fund performance insights
## Dashboard
![Screenshot 2025-05-25 232855](https://github.com/user-attachments/assets/f95af37b-0385-49fd-bfa5-3205fa7780bc)
## Project Insights:
- Over 65% of mutual funds showed positive YTD returns.
- Most daily change percentages lie between 0.00% to 0.05%, indicating moderate daily movement.
- VUIAX, VYMUX, and WIINX are top funds by current price distribution.
- Average 3-month return and 52-week change % show steady fund performance with moderate volatility.
- The relationship between price and daily change % is scattered but generally low for lower-priced funds.
## Project Description:
- This project involves the complete end-to-end pipeline of financial data analysis using public mutual fund data. Starting with web scraping mutual fund gainer data from Yahoo Finance, the raw HTML was parsed using Python (BeautifulSoup). The data was cleaned using Pandas, with transformations applied to extract meaningful numerical formats.
- Once cleaned, the dataset was imported into Power BI, where KPIs were calculated using DAX formulas. A dashboard was built to present financial metrics, return trends, and price distributions through line charts, bar charts, stacked visuals, and KPI cards. The resulting visuals and metrics help users assess which funds are performing well and how their metrics compare across key indicators like price, return %, and volatility.
