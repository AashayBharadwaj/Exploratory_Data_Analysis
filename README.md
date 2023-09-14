# Exploratory_Data_Analysis

Description of project

>Implemented an ETL pipeline to extract, transform and load data from various sources using their respective APIs into a central database using SQL server, enabling efficient and accurate data analysis.
>Performed complex SQL queries to generate insights on various factors that affect the price of a particular crypto. 
>Leveraged tableau to illustrate the valuable insights generated from the analysis.

	
Phase 1 of the project.

Data Extraction.
We scraped data from different websites using their APIs. 
Here’s the list of websites used:
1)	https://coinmarketcap.com/
2)	https://etherscan.io/
3)	https://snowtrace.io/
4)	https://bscscan.com/

Using these websites, we generated numerous csv files regarding different data points. 
The challenge we faced with the data that we received was that we had a lot of inconsistent, redundant data and had a lot of missing values. 
So, this data could not be directly used for data analysis.  It needed to be processed.

Phase 2 of the project.
(Data Transformation)	
To overcome the challenge mentioned above, we had to perform data cleaning where we got rid of the redundant and unnecessary data. 
After this the data was in a condition to be worked on.


![Screenshot_20220612-192627__01](https://github.com/AashayBharadwaj/Exploratory_Data_Analysis/blob/main/ERD_.jpg)



![Screenshot_20220612-192627__01](https://github.com/AashayBharadwaj/Exploratory_Data_Analysis/blob/main/Physical_Data_Model.jpg)


Physical Data Model
We used SQL developer. We used queries to create tables. We have also used constraints and defined primary keys.
One key challenge was that for our dataset we had time series data repeating for different blockchains. 
To overcome this, we had to introduce an artificial PK to uniquely identify rows.

Phase 3 of the project.
 
(Data Loading Concept Used) 
Data loading has been done in three parts: Extraction, Transformation, and Loading. 
Extraction: We extracted data using APIs from different websites like coinmarketcap, etherscan, snowtrace, defilama. 
We got csv files from these websites which were used for our analysis.
Transformation: 
We transformed data by performing tasks like data cleaning, removing redundant and unnecessary columns, 
handling missing values, and made the data consistent.

Loading: For loading the data we used SQL developer which is a very powerful tool for working on structured data. 
It provides various functionalities through which we can manage the data at an optimal level.

Once the transformation step is done, we created the required tables which are logically related to each other with a defined relationship between them.



Phase 4 of the project. (Data Analysis and Visualization) With the clean and structured data in our SQL database, we proceeded to analyze it to gain valuable insights into the factors affecting the price of cryptocurrencies. Complex SQL queries were employed to perform various analyses, including trend analysis, correlation studies, and anomaly detection. These analyses helped us identify patterns and relationships between different crypto assets and external factors such as market sentiment, trading volume, and blockchain activity.

To present our findings effectively, we utilized Power BI, a powerful data visualization and business intelligence tool. Power BI allowed us to create interactive and dynamic dashboards and reports that showcased our insights in a visually compelling manner. We designed custom dashboards with various charts, graphs, and heatmaps to provide a holistic view of the cryptocurrency market. This visualization not only made it easier to interpret our findings but also enabled stakeholders to make data-driven decisions in real-time.

As an example of how factors like daily active users can affect the price of Ethereum (ETH), let's consider a scenario:

Suppose we are analyzing the price movement of Ethereum (ETH). In our dataset, we have historical data on Ethereum's price, trading volume, and daily active users of its associated blockchain platform. Using Power BI, we create a dashboard that includes the following visualizations:

Price Trend Chart: A line chart that displays the historical price of Ethereum (ETH) over time.
Daily Active Users (DAU) Chart: A bar chart showing the number of daily active users on the Ethereum blockchain platform.
Trading Volume Chart: A bar chart illustrating the daily trading volume of Ethereum.
Upon analyzing these visualizations, we notice a correlation between the price of Ethereum and its daily active users. Here's how this correlation could work:

Scenario 1 - Positive Correlation: In periods where Ethereum experiences a significant increase in daily active users, we observe a corresponding uptrend in its price. This suggests that a growing user base may generate increased demand for Ethereum, driving its price higher. Investors and traders notice this positive trend, leading to further investment and price appreciation.

Scenario 2 - Negative Correlation: Conversely, during periods of declining daily active users, we notice a decrease in Ethereum's price. A shrinking user base could signal reduced interest or adoption, which may lead to decreased demand and a lower price. This can trigger sell-offs and further price declines.

By visualizing these relationships in Power BI, stakeholders can quickly grasp how daily active users influence the price of Ethereum, enabling them to make informed decisions based on this key factor. This real-time insight is invaluable for cryptocurrency investors and blockchain project managers seeking to understand and respond to market dynamics.

![Screenshot_20220612-192627__01](https://github.com/AashayBharadwaj/Exploratory_Data_Analysis/blob/main/ETH_PRICE_VS_ACTIVE_USERS.png)







