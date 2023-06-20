# Phase_4_project
# Title 
A Time Series Analysis of Real Estate Prices in Top 5 Zip Codes"

# Project overview <br>
In these project we shall seek to do the following :

* Load the dataset
* Understand the dataset
* Choose our target variable.
* Prepare the dataset (Example : Cleaning the dataset , checking for multicollinearity)
* Encode our categorical variables
* Make several models
* Evaluate our models
* Use our models for prediction
* Come up with relevant findings.
* 
 # Main Objective <br>
* The main objective of this project is to identify the top 5 zip codes that offer the best investment potential in terms of real estate prices. By analyzing historical trends and patterns, the project aims to provide actionable insights to the investment firm, enabling them to make informed decisions on where to allocate their resources.

# Specific Objectives <br>
1. Analyze Historical Data: The project involves analyzing the historical data of real estate prices across different zip codes. This includes understanding the trends, patterns, and fluctuations in property values over time.

2. Identify Promising Zip Codes: Using the analysis of historical data, the project aims to identify the zip codes that have shown consistent growth, stability, or potential for future appreciation. These zip codes are considered the most favorable for investment.

3. Consider Location Factors: In addition to the historical performance, the project also takes into account location-specific factors such as city, state, and metro. This information helps assess the overall desirability and attractiveness of the investment opportunities.

4. Evaluate Market SizeRank: The SizeRank attribute provides insights into the relative size and competitiveness of the real estate market in each zip code. This factor helps gauge the potential opportunities and risks associated with investing in a particular area.

#  Data Understanding

The dataset contains information on various attributes, including RegionID, RegionName, City, State, Metro, SizeRank, CountyName, and value (real estate prices). Our dataset is the Zillow Housing Dataset which was sourced from Zillow Research Page.<br>
## Column Name	Description
* RegionID -This is unique Id for the Regions<br>
* SizeRank -This is the ranking done based on the size of the region<br>
* RegionName -	This field contains the zip code of the region.<br>
* RegionType-	Type of region is Zip.<br>
* StateName	- State<br>
* City	- This column provide the specific City Name of Housing Data<br>
* Metro	- This provide the name of the metro city around that region<br>
* County Name	- This is the county name for that region<br>
* Months Column	- These columns contains the prices of region for every month<br>

# Libraries
* PYTHON- Programming language
* PANDAS- Exploratory data analysis
* SEABORN- Visualization
* NUMPY - Numerical computing and data analysis
* MATPLOTLIB- Visualization
* STATSMODELS-statistical analysis and modeling
* SCIKIT LEARN- machine learning
* SCIPY- scientific computing
* MATH- basic mathematical operations
* 
# Exploratory Data Analysis
![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/8fe0337e-7f1c-467a-bb50-8b07ee836a9f)


![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/eb6640b7-72c5-499b-acc1-ef1c5256ad53)



![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/977d46fe-cc69-46be-8acd-439750b7506c)


![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/868ff9c0-8cde-46e7-845e-8cbbaf859c0a)


![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/591be7bc-d5f6-4450-96c1-e8aa72e3c31c)

# Modelling

## ACF & PACF

![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/7af45f54-a62c-4893-9d89-d2ea0abf34b8)


![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/08641225-73aa-4a75-babb-2e207ca2fc2a)

# Forecasts

![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/44b5c80f-51b9-4490-be03-0bca148295ae)


![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/a996e237-66dd-423d-87cc-32be939245ad)


![image](https://github.com/rotichnaomi/Phase_4_project/assets/122217304/c01ece0f-4a40-4877-9298-98a962b8fa4e)


 # Findings

 # Findings

After performing a time series analysis on the 10 zip codes and forecasting total returns for up to three years, we recommend the company invest in the following 3 zip codes:

* 81611 - Location: Aspen, CO             (R.O.I - 132.378817)

* 10021 - Location: New York, NY          (R.O.I - 111.795552)

* 34102 - Location: Naples, FL            (R.O.I - 7.605307)


As for the other 6 zip codes, they are not fit for investment given the negative returns.

# Recommendations

We recommend investing in the following regions :

* 81611 - Location: Aspen, CO     

* 10021 - Location: New York, NY   

* 34102 - Location: Naples, FL 

This is because these regions have positive returns on investments, unlike the other areas.






