# PHASE 4 PROJECT: REAL ESTATE TIME SERIES ANALYSIS.
# **1). Business Understanding**


Real estate investment is a lucrative and dynamic industry that requires careful analysis and decision-making. The fictional real estate investment firm is seeking guidance on identifying the top 5 zip codes for investment opportunities. To address this question, historical data from Zillow Research is utilized.
## **i) Background:**

Real estate investment is a lucrative and dynamic industry that requires careful analysis and decision-making. The fictional real estate investment firm is seeking guidance on identifying the top 5 zip codes for investment opportunities. To address this question, historical data from Zillow Research is utilized. The dataset contains information on various attributes, including RegionID, RegionName, City, State, Metro, SizeRank, CountyName, and value (real estate prices).

## **ii). Main Objective:**

The main objective of this project is to identify the top 5 zip codes that offer the best investment potential in terms of real estate prices. By analyzing historical trends and patterns, the project aims to provide actionable insights to the investment firm, enabling them to make informed decisions on where to allocate their resources.

### **Specific Objectives:**

* Analyze Historical Data: The project involves analyzing the historical data of real estate prices across different zip codes. This includes understanding the trends, patterns, and fluctuations in property values over time.

* Identify Promising Zip Codes: Using the analysis of historical data, the project aims to identify the zip codes that have shown consistent growth, stability, or potential for future appreciation. These zip codes are considered the most favorable for investment.

* Consider Location Factors: In addition to the historical performance, the project also takes into account location-specific factors such as city, state, and metro. This information helps assess the overall desirability and attractiveness of the investment opportunities.

* Evaluate Market SizeRank: The SizeRank attribute provides insights into the relative size and competitiveness of the real estate market in each zip code. This factor helps gauge the potential opportunities and risks associated with investing in a particular area.

  # **2)**. **Data Understanding**

The dataset contains information on various attributes, including RegionID, RegionName, City, State, Metro, SizeRank, CountyName, and value (real estate prices). Our dataset is the Zillow Housing Dataset which was sourced from Zillow Research Page.
## Column Name	Description
* RegionID -This is a unique Id for the Regions<br>
* SizeRank -This is the ranking done based on the size of the region<br>
* RegionName -	This field contains the zip code of the region.<br>
* RegionType-	The type of region is Zip.<br>
* StateName	- State<br>
* City	- This column provides the specific City Name of Housing Data<br>
* Metro	- This provides the name of the metro city around that region<br>
* County Name	- This is the county name for that region<br>
* Months Column	- These columns contain the prices of the region for every month<br>

In order to understand what our dataset looks like let us get a preview of this data by loading it.
## **3). Data Preparation**
This is to make the data in a format that is good to feed to our model. It involves the following series of steps:<br>
* Cleaning the data<br>
* Checking for and dealing with missing values<br>
* Reshaping our dataset from wide to long format<br>
  # 4). Exploratory Data Analysis
  This is basically trying to figure out more about our data, its behaviors, and patterns
  This involves the following:<br>
  * Grouping the data by month.

    ![Read Me monthly Eda](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/94025eda-57c4-4d90-88b1-45ee2fda561e)

  * Group the data yearly.

    ![Eda Yearly plot](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/640741c3-0b51-42fe-8224-55f09e25970f)
* Grouping per quarter and plotting.

  ![quarterly plot](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/419a39da-127a-4022-a6dc-d56a126a3dc8)
  * Grouping per decade

![Eda per decade](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/d42ade3e-12ee-4f54-a18a-de11d1f4685b)
  *  Finding the top 5 Best regions

  Here we seek to find the five best regions by using the return on investment, where high returns show the best regions. Below is a plot of our findings

  ![ROI](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/8808016c-6de8-4e97-8c8a-09a75de545fd)
  * Checking for trends and seasonality
    Here we seek to find the relevant trends in the dataset, based on the best regions, below are our plots

    ![Line plot](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/8be22aa7-0b70-41aa-a581-e49687592fd7)
    * Checking for the rolling statistics <br>
    * Performing Dullers test. <br>
    * Checking for stationarity <br>
    * Detrending our dataset <br>
    * Deseasonalizing our dataset <br>
    * Performing Seasonal decomposition <br>
    ## **5). Modeling**
    This is now creating various models to forecast our data. we created the following models :
    * ARIMA modelels <br>
    *  SARIMAX models. <br>
    *  PROPHET models. <br>
      First, we plot the auto-correlation plots, then we do the modeling.
1. **Arima Models** <br>
 We created an Arima model, below are the statistical results.<br>
   <img width="553" alt="Arima" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/c7a99ee9-2f65-4486-8512-1f8dfa89a7a5">
2. **Sarimax Models**<br>
Below is the statistical result using the Sarimax models.

<img width="586" alt="Sarimax" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/75da97a4-b36d-409f-899d-910667e9e3d1">

Below is a plot of the actual and predicted values of our Sarimax model with a 1.94 RMSE <br>

![Sarimax](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/627564a9-335e-471a-909a-d45ef0d31f11)
3. ** Prophet Models**
We used this model to forecast and predict values, below are some of  our predicted values (**Note: The yhat means the predicted values**)  <br>
<img width="257" alt="Prophet model" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/13c9cebc-349b-4165-8c0c-c8a7f97a2028">

   ## 7). Summary
   After performing a time series analysis on the 10 zip codes and forecasting total returns for up to three years, we recommend the company invest in the following 3 zip codes:

* 81611 - Location: Aspen, CO             (R.O.I - 132.378817)

* 10021 - Location: New York, NY          (R.O.I - 111.795552)

* 34102 - Location: Naples, FL            (R.O.I - 7.605307)


As for the other 6 zip codes, they are not fit for investment given the negative returns.
