# Project Background 

TimmyDEPOT, established in 2011, is an American e-commerce retailer and business-to business sales organization that sells popular office supplies, furnitures and technology products via its website across the U.S., 

The company has significant amounts of data on its sales and product offerings from 2011 and 2014. This project thoroughly analyzes and synthesizes this data in order to provide a global performance overview but also uncover critical insights that will imporve TimmyDEPOT's commercial success. 

Insights and recommendations are provided on the following key areas: 
- Sales Trends Analysis : Evalutaion of historical sales patterns, at every granularity, focusing on Sales, Margin, Sales Volume and Order Volume.
- Product Level Performance : An analysis of TimmyDEPOT's various product lines, understanding their impact on sales and returns. 	

A dynamic and interactive Power BI dashboard can be downloaded [here](https://drive.google.com/file/d/1tJmYqvQg9Wl8GgzIBcImNzqPXngob_Pa/view?usp=drive_link) and opened in PowerBI. A PDF version (not interactive) is also available [here](https://github.com/user-attachments/files/17345541/TimmyDepotSales.pdf).

Different slicers are located in the top right of the dashboard pages. 
Please, do not hesitate to interact with the visuals by hovering or clicking the many points of interest to display additional relevant information or perform dynamic slicing. 

The list of all the dax queries used to create the calculated measures and KPIs can be downloaded [here](https://docs.google.com/document/d/1opihpei_4-dEf88gOMW8lWPRbwRCYGQ-_mbCmQ-sb9Y/edit?usp=sharing).

# Data Structure & Initial Checks 

TimmyDEPOT's dataset consisted of one singular excel table. It then has been processed in the Power BI's Power Query Editor in order to transform it into a star schema structure. The processed data model structure, as seen below, consists of four dimension tables (DimGeo, DimCustomer, DimProduct and DimDate) and one fact table (FactsSales) with a total row count of 15,105 records.

<img width="489" alt="image" src="https://github.com/user-attachments/assets/91f3852d-1fc6-47c3-9454-4bafa5aab36e">

Prior to beginning the analysis, a variety of checks were conducted in the Power Query Editor for quality control but also familiarization with the datasets, including the exploration of value distribution and profiling of every columns. 

# Executive Summary

## Overview of findings 

Despite a slight decrease in early 2012, **the company's sales have continued to increase over the years**. Key performance indicators such as **Sales**, **Items sold** and **Order Volume** have all followed **the same dynamic of a significant increase throughout the months of a year into a massive drop at the begining of the following year**. Unlike the other metrics, **profit seems to follow an independent dynamic**. The following sections will explore contributing factors and highlights key opportunity areas for improvement. 

Below is the summary page from the Power BI report and more examples are included throughout the report. The entire interactive dashboard can be downloaded [here](https://drive.google.com/file/d/1tJmYqvQg9Wl8GgzIBcImNzqPXngob_Pa/view?usp=drive_link).

![image](https://github.com/user-attachments/assets/254308e7-d34d-45f3-bc8f-f7dcbf562468)


### Sales Trends : 

- The company has seen its **annual sales increase over the years**, totalling 2,30M€  at the end 2014.
Order Volume has followed the same trend to reach a total of 9993 order placed.

- Despite the overall upward trend, **the company's sales recorded its only YOY decrease in 2012** (-2.8%), due to a relatively poor performance in comparison with the strongs 1Q2011 and 3Q2011 that recorded unusually high sales of machine products. Yet, **2012 YOY profit recorded a signicant increase (+24,3%)** of which the reasons will be highlighted in the product performance section. 

![image](https://github.com/user-attachments/assets/c902f799-155e-4905-acd3-1b5588cb8074)


- Nevertheless, **the sales metrics kept following the same pattern at a yearly level** : a steep increase over the quarters into a significant decrease at the start of the next year. A possible explanation is that the order volume (which is obviously highly correlated with the sales metrics) is significantly impacted by the dynamics of the calendar year, especially for the types of product sold such as office supplies and furnitures. 

- **YOY profit shows a very high variance** (+143% in 1Q2012 and +90% in 1Q2014 for example) unrelated with the other metrics. Let's discover why with the product performance breakdown.

![image](https://github.com/user-attachments/assets/06ee0066-64d8-473d-b96c-a813b2fdc82d)

### Product performance 

- **All-time Sales are evenly spread accross the three category of products**. Yet **the furniture category is poorly performing in terms of Profit** compared to the others with an **all-time average margin of 3.88%**. 

![image](https://github.com/user-attachments/assets/34cd42c3-3ed0-4c53-82e9-3b7afc1f5b88)


- **The 3 product categories increased its YOY sales over the years** except for 2012 where **a slight decrease was recorded for the Office supply and Technology categories** (respectively -10% and -7%). It can attributed to a **slight decrease in the order volume of high base price products**.

- **Profit**, which is a crucial metric, is highly **impacted by the base margin and the discount applied**. Indeed, a high margin product can be significantly discounted more than a low margin product without risking negative product.
Indeed, as previously said, the **furniture category contains product with particularly low base margin while the office supplies category contains several products with exceptionaly high base margin %**. With an average discount applied above the two others categories over the years, **the furniture category only accounts for 6% of the all-time profit total**. 

![image](https://github.com/user-attachments/assets/d9272a92-4f09-4efd-ba8d-d98b4dfb2540)


- **The company reached its highest monthly profit (18k€) in December 2014**, where the binders product (44% average margin across this sub-category of products) accounted for 40% of the total and the average discount across all categories was relatively low (~13%).

![image](https://github.com/user-attachments/assets/958d93b0-8118-4798-8dbf-c8a16e2b796a)

# Recommandations 

Based on the uncovered insights, the following recommandations have been provided :

- To counter the recurring weak beginning of each year, it is crucial to aim at increasing the **overall order volume during this period, especially for the first quarters while maintaining a good margin %.

- Consider conducting a **dedicated marketing campaign for this time period including aggressive discounts**. Nevertheless, the products targeted need to have a **high enough base margin value** such as binders (44%) and copiers (43%) in order to prevent negative profit.

- On the other hand, consider **reducing the discounts for products with very low base margin** even if it means a decrease in order volume. For example, furniture products have been barely profitable so far (6% of overall profit) but also other products like machines are often not generating any benefits. 
