# sales-Forecasting-model-

link to the model - https://share.streamlit.io/jahanshah1/sales-forecasting-model-/main/final.py

## Introduction
This is an ARIMA (Auto Regressive Integrated Moving Average) model to predict the sales of a business or a product with a user friendly graph plot, It can help predict future sales based on the historical data given in `.csv` format.  

## screenshots 
### main-page
<img width="1440" alt="Screenshot 2022-06-12 at 11 16 41 AM" src="https://user-images.githubusercontent.com/92823408/173217752-c69263ca-2b43-40e0-b995-0521db6aa1a6.png">
homepage of the model, where the raw predicted data is shown and 'years of prediction' is selected 

### Plot
<img width="988" alt="Screenshot 2022-06-12 at 11 16 50 AM" src="https://user-images.githubusercontent.com/92823408/173217837-e250006a-e7ef-41a2-8e3c-6a6fabaa9cc2.png">
Here the raw data is plotted into a graph so people can understand it better. The black dots refer to the actual data (a constant), the blue line is the predicted value and the blue area hovering around the blue line is the expected loss of accuracy.

### forecast components
<img width="829" alt="Screenshot 2022-06-12 at 11 17 02 AM" src="https://user-images.githubusercontent.com/92823408/173218413-dd311d83-62b7-48a9-a024-58b0029b8464.png">
Some components to help viewers understant the trend better 


## Tech stack used 
- Python 
- Streamlit 
- FBProphet 
- Pandas 

## Overview
Forecasting is a common data science practice which helps organisations to set their goals/plans. This model essentially helps an organization in anomaly detection and setting goals. This model works best with saturated markets but can also be used with volatile markets. Uncertainity in a forecast is estimated by extending the generativemodel forward. The generative model for the trend is that there are `S`  changepoints over a history of `T` points,  each of which has a rate change `jLaplace(0;)`.

### Seasonality 
Business time series often have multi-period seasonality as a result of the human behaviors they represent. For instance, a 5-day work week can produce effects on a time series that repeat each week, while vacation schedules and school breaks can produce effects that repeat each year.  To fit and forecast these effects we must specify seasonality models that are periodic functions of `t`.

## Running the model
In order to view/test the project you can directly click on the link mentioned above. But if you want to add your own historical data (.csv) for prediction then the user will need to download the project and change the current `.csv` with your historical data and in `df` variable they will need to input the name of their historical data file and run `final.py`



