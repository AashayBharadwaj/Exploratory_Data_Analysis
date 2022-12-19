# Exploratory_Data_Analysis

Description of project

A cryptocurrency is a digital currency, which is an alternative form of payment created using encryption algorithms. 
The use of encryption technologies means that cryptocurrencies function both as a currency and as a virtual accounting system. 
Due to its wide range of use cases it is getting adopted at a tremendous rate. In this project we are doing exploratory data analysis on cryptocurrencies.
We gathered data from various sources regarding different cryptocurrencies and analyzed them based on various factors. 
The points we explored are different blockchains, price data of different cryptocurrencies, daily active users, and popularity of different blockchains.
	
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

<img src="\Users\aasha\OneDrive\Desktop\Physical_Data_Model.jpg" alt="Alt text" title="Optional title">


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
