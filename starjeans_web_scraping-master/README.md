# Welcome to the Star Jeans Data Analysis  
![alt text](img/starjeans.jpg?raw=true)  

---

## 1 - Business Problem  

Eduardo and Marcelo are two Brazilian friends and business partners. After several successful ventures, they are planning to enter the U.S. fashion market with an E-commerce business model.  

The initial idea is to start with just one product for a specific audience. The product will be men's jeans, with the goal of keeping operational costs low and scaling as they gain customers.  

However, even with the product and target audience defined, the two partners lack experience in the fashion market and therefore cannot determine basic details such as pricing, jeans type, and materials required for production.  

Thus, the two partners hired a Data Science consultancy to answer the following questions:  
1. What is the best selling price for the jeans?  
2. How many types of jeans and colors should be offered initially?  
3. What raw materials are necessary to manufacture the jeans?  

---

## 2 - Data Overview  

| Attribute        | Description                                                  |  
|------------------|--------------------------------------------------------------|  
| product_id       | Unique ID for each product.                                  |  
| style_id         | Unique ID for each style.                                    |  
| color_id         | Unique ID for each color.                                    |  
| product_name     | Name of the product.                                         |  
| color_name       | Name of the color.                                           |  
| fit              | Jeans fit type.                                              |  
| product_price    | Product price.                                               |  
| cotton           | Percentage of cotton in the jeans.                           |  
| polyester        | Percentage of polyester in the jeans.                        |  
| spandex          | Percentage of spandex in the jeans.                          |  
| scrapy_datetime  | Date when the data was collected.                            |  

> **The data was collected from H&M's website (one of the largest clothing companies).**  

Website link: [H&M Website](https://www2.hm.com/en_us/men/products/jeans.html)  

---

## 3 - Solution Strategy  

**3.1 Data Collection:**  
Perform web scraping on H&M's website (automated collection of structured web data). The library Beautiful Soup was used for web scraping.  

Library link: [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)  

**3.2 Data Cleaning:**  
This stage used Regex (Regular expressions, or Regex, are patterns used to identify specific character combinations in a string) and other techniques to separate, correct, and clean the collected data.  

**3.3 ETL Design:**  
ETL (Extract, Transform, Load) is a structured process for extracting data from various systems, transforming it per business rules, and loading it into a data warehouse.  

- Design the ETL architecture.  
- Order dependencies between jobs (tasks), as some depend on others.  
- Schedule and automate jobs using Cron, which runs ETL processes in the background.  
- Implement a logging system to monitor ETL behavior and identify issues, such as where a data collection process failed.  

<img src="img/arquitetura_de_etl.png" width="600">  

**3.4 Database Creation:**  
Create a SQLite table with the collected data.  

**3.5 Data Analysis:**  
Perform statistical analysis for each attribute in the collected dataset.  

**3.6 Data Visualization:**  
Generate graphs related to key business problems for better data understanding.  

**3.7 Create Dashboard:**  
Using the Panel library, create a dashboard displaying project results.  

<img src="img/dashboard.png" width="600">  

---

## 4 - Business Results  

**4.1 - Median Prices of Popular Products:**  

| Index | Product                | Price (US$) |  
|-------|------------------------|-------------|  
| 1     | Slim Jeans             | 19.99       |  
| 2     | Skinny Jeans           | 19.99       |  
| 3     | Regular Jeans          | 19.99       |  
| 4     | Freefit® Slim Jeans    | 34.99       |  
| 5     | Trashed Skinny Jeans   | 24.99       |  

**4.2 - Most Popular Colors:**  

| Index | Color              |  
|-------|--------------------|  
| 1     | Denim Blue         |  
| 2     | Light Denim Blue   |  
| 3     | Black              |  
| 4     | Dark Denim Blue    |  
| 5     | Dark Gray          |  

**4.3 - Final Dashboard:**  
<img src="img/dashboard_final.png" width="1000">  

Notebook with dashboard: [Notebook](final_data_analysis_dashboard.ipynb)  

---

## 5 - Conclusions  

You may have heard that "Data is the new oil." With web scraping, we gain access to data. With the collected data, we can monitor market trends, gather information to attract new customers, make forecasts, and much more.  

Raw data, however, is not easy to interpret, which is where ETL comes in. It cleans and prepares the data, enabling companies to base decisions on concrete insights rather than intuition.  

---

## 6 - Next Steps to Improve  

- Collect data about sizes.  
- Gather information on competitors.  
- Collect data over a more extended period to capture seasonality trends.  

---

## 7 - Technologies  

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)  
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)  
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)  
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)  
![PyCharm](https://img.shields.io/badge/pycharm-143?style=for-the-badge&logo=pycharm&logoColor=black&color=black&labelColor=green)  
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)  
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)  

---

## 8 - Author  

## 6. Contact

Vaishnavi Tripathi
Data Scientist

[Project Portfolio](https://ttripathi167.github.io/Portfolio/)

[GitHub Profile](https://github.com/ttripathi167/) 

