# Project-Sales-Dashboard
The data, content, and final delivery I shared on GitHub utilize mock-up data due to confidentiality. This work sample aims to demonstrate my analytical skills, problem-solving approach, and the lessons I learned from the case.

### Table of contents
* [1. Introduction](#1)
* [2. Specifications](#2)
* [3. RFM Dashboard Proof of Concept](#3)
* [4. Dataset](#4)
* [5. Model Simulation](#5)
* [6. Results](#6)
    * [Proof of Concept Dadhboard Design](#6.1)
    * [Design Considerations - Assumptions](#6.2)
    * [Technical Challenges - Highlights](#6.3)
    * [Business Insights - Recommendations](#6.4)
    * [Lesson Learned](#6.5)

![image.jpg]()

<a id="1"></a>
### 1. Introduction

The objective of this solution delivery is to model, measure, analyze and track the status of sales within this furniture department store. 

<a id="2"></a>
### 1. Specifications
The dashboard consists of three pages, 

<a id="4"></a>
### 4. Dataset
The dataset consists of a total of 9 tables, including 3 source data tables and 6 data mart tables.<br />
<br />
**Orders:**  This fact table contains information such as customer code, order code, order date, postal code, last product update, and product code  <br /> 
<br />
**People:** Provides information about person (cutomer name) and regions<br />
<br />
**Returns:** Contains data on order codes and indicates whether a product has been returned<br />
<br />
**Calender:** Includes a single record for each date used in the analysis<br />
<br />
**Customer:** Generated from the order table, it includes details such as customer code, customer name, and segment<br />
<br />
**Date Type:** Specifies the type of date, either order date or ship date<br />
<br />
**Last Refresh:** Each time the dashboard is refreshed, this table updates and returns the latest refresh time<br />
<br />
**Product:** Generated from the order table with a predefined filter, it includes product details such as product code, category, sub-category, product name, and last product update<br />
<br />
**Region:** Generated from the order table, this table contains information about postal code, country, state, city, and region<br />
<br />







<a id="6"></a>
### 6. Results
<a id="6.1"></a>
#### Proof of Concept Dadhboard Design
![image.jpg](https://github.com/christychen65/Case-Marketing-Campaign-CRM-RFM-Dashboard/assets/132826012/b44922a4-a2e8-4a19-8392-b782eed489d1)
![image.jpg](https://github.com/christychen65/Case-Marketing-Campaign-CRM-RFM-Dashboard/assets/132826012/03442485-4bad-4415-81e4-1eed16872dfc)
![image.jpg](https://github.com/christychen65/Case-Marketing-Campaign-CRM-RFM-Dashboard/assets/132826012/e313ac08-b596-41c6-9cea-6315579f7065)
![image.jpg](https://github.com/christychen65/Case-Marketing-Campaign-CRM-RFM-Dashboard/assets/132826012/390ea03c-368d-45ce-b569-9f39ddc669c2)
<br />
<a id="6.2"></a>
#### Design Considerations - Assumptions
1> SCD: Product<br />
2> Postcode as Primary Key in Region hierarchy<br />
3> Data Security, Region manager should see specific regional KPIs based on their logins
<br />
<a id="6.3"></a>
#### Technical Challenges - Highlights
1> Parameterized environmental variables for future deployment<br />
2> Parameterized Time table in M code for general and fiscal calendars<br />
3> M code to address latest refresh time<br />
4> Created functions for various purposes
<br />
<a id="6.4"></a>
#### Business Insights - Recommendations
1> Profit Rate is very useful for product purchasing and pricing strategy<br />
2> By analyzing customers shopping habit and their GM (%), CRM team can easily plan campaign targeted specific customers<br />
3> Return Rate is a useful KPI for product team to make product plan
<br />
<a id="6.5"></a>
#### Lesson Learned
