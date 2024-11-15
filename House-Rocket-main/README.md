# House Rocket Analytics

![King County Map](https://github.com/jlcunha/House-Rocket/blob/main/imagens/KingCounty.jpg?raw=true?raw=true)

This project is a data science simulation for a real estate company. As a result of this project, we addressed several information management problems and managed to increase the company's profit margin by a total of **19.89%**.

---

## 1. About the Project

### 1.1 Business Problem

House Rocket is a (fictional) real estate company that operates in **King County, USA**, buying and selling properties to generate profit.  

The company faces several challenges, such as:

- They need to conduct analyses independently.  
- They are not fully utilizing their dataset to uncover valuable insights.  
- They lack clarity on which houses to buy or sell and at what price.  

---

### 1.2 Data Overview

| **Attribute**    | **Description**                                                                 |
|-------------------|---------------------------------------------------------------------------------|
| `id`             | Unique identifier for each property.                                            |
| `date`           | Date the property was added to the dataset.                                     |
| `price`          | Asking price for the property.                                                  |
| `bedrooms`       | Number of bedrooms.                                                             |
| `bathrooms`      | Number of bathrooms.                                                            |
| `sqft_living`    | Living area size in square feet.                                                |
| `sqft_lot`       | Lot size in square feet.                                                        |
| `floors`         | Number of floors.                                                               |
| `waterfront`     | Binary variable indicating if the property has a waterfront view.               |
| `view`           | Quality of the property's view (scale: 0-4).                                    |
| `condition`      | Property's overall condition (scale: 0-5).                                      |
| `grade`          | Construction quality and architectural standard (scale: 1-13).                 |
| `sqft_above`     | Above-ground area size in square feet.                                          |
| `sqft_basement`  | Basement area size in square feet.                                              |
| `yr_built`       | Year the property was built.                                                    |
| `yr_renovated`   | Year the property was last renovated.                                           |
| `zipcode`        | Property's postal code.                                                         |
| `lat`            | Latitude.                                                                       |
| `long`           | Longitude.                                                                      |
| `sqft_living15`  | Average living area size of the 15 nearest neighbors.                           |
| `sqft_lot15`     | Average lot size of the 15 nearest neighbors.                                   |

[Dataset from Kaggle](https://www.kaggle.com/harlfoxem/housesalesprediction)  
![Kaggle Badge](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

---

### 1.3 Solution

#### **1.3.1 Analytical Application**  
An interactive dashboard deployed on **Heroku**, enabling users to conduct their analyses.

<img src="imagens/dashboard1.png" width="600">
<img src="imagens/dasboard2.png" width="600">

[House Rocket App](https://dados-house-rocket.herokuapp.com/)  
![Heroku Badge](https://img.shields.io/badge/heroku-%23430098.svg?style=for-the-badge&logo=heroku&logoColor=white)

---

#### **1.3.2 Insights**  
Insights generated through data visualization are summarized below. For detailed insights, refer to the [Jupyter Notebook](https://github.com/jlcunha/House-Rocket/blob/main/house_rocket.ipynb).

![Dashboard Insights](https://github.com/jlcunha/House-Rocket/blob/main/imagens/Dashboard.jpg?raw=true?raw=true?raw=true)

---

#### **1.3.3 Property Purchase and Sales Recommendations**  
A report listing properties to buy and recommended selling prices was created based on these conditions:

- Property price per square foot must be **below the median** price per square foot for its region (`zipcode`).  
- Property condition must be **3 or above**.

[Download Report (casas_para_compra.csv)](https://github.com/jlcunha/House-Rocket/blob/main/casas_para_compra.csv)

---

#### **1.3.4 Financial Impact of Recommendations**  

- **Total purchase cost**: \$5,163,360,430.  
- **Potential profit**: \$1,026,992,389 (**19.89% profit margin**).  

To optimize operations, the report recommends starting with properties that have a **condition and view rating of 4 or higher**, as these are more attractive for marketing campaigns and easier to sell.

---

## 2. Technologies Used
- **Python 3**
- **PyCharm**
- **Jupyter Notebook**
- **Streamlit**
- **Heroku Cloud**

---

## 3. Project Files
- [Jupyter Notebook Codes](https://github.com/jlcunha/House-Rocket/blob/main/house_rocket.ipynb)  
- [Heroku App Files](https://github.com/jlcunha/House-Rocket/tree/main/HerokuApp)  

---

## 4. Next Steps
- Design and execute tests to isolate causes and effects.  
- Recommend strategy or expenditure changes to improve results.  
- Identify customer and prospect groups for targeted insights.

---

## 5. Acknowledgements
This project is part of the course *Python: From Zero to Data Scientist* - [Comunidade DS](https://www.comunidadedatascience.com/comunidade-ds/).

---

## 6. Contact

Vaishnavi Tripathi
Data Scientist


[Project Portfolio](https://ttripathi167.github.io/Portfolio/)

[GitHub Profile](https://github.com/ttripathi167/)
