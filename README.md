# sales-Forecasting-model-

link to the model - https://share.streamlit.io/jahanshah1/sales-forecasting-model-/main/final.py

## Introduction
This is an ARIMA (Auto Regressive Integrated Moving Average) model to predict the sales of a business or a product with an user friendly graph plot, It can help predict future sales based on the historical data given in `.csv` format.  

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
Forecasting is a common data science practice which helps organisations to set their goals/plans. This model essentially helps an organization in anomaly detection and setting goals. This model works best with saturated markets but can also be used with volatile markets. Uncertainity in a forecast is estimated by extending the generative model forward. The generative model for the trend is that there are `S` changepoints over a history of `T` points,  each of which has a rate change `jLaplace(0;)`.


### Seasonality 
Business time series often have multi-period seasonality as a result of the human behaviors they represent. For instance, a 5-day work week can produce effects on a time series that repeat each week, while vacation schedules and school breaks can produce effects that repeat each year. To fit and forecast these effects we must specify seasonality models that are periodic functions of `t`.

## Purpose
The main purpose of this model is to help every business/organisation to utilise ML models easily, I have created a User friendly web app so even a non-techy person can make the most out of Machine Learning! The ultimate goal is to create a web app in which the user can have various option of selecting ML/AI models based on their accuracy for prediction. 

## Running the model
In order to view/test the project you can directly click on the link mentioned above.

### simply running the model in local host:
- download the file from github
- run `final.py`
- input `streamlit run final.py` in the terminal

But if you want to add your historical data then you will need to follow these steps:
- download the file from github 
- change `AirPassengers.csv` with your `.csv` containing the historical data (the data should be in two columns with date and closing value)
- In the `df` variable change `AirPassengers.csv` with your path of the data 
- In `df_train = df[['Month','#Passengers']]` and `df_train = df_train.rename(columns={'Month':'ds','#Passengers':'y'})` swap "month" and "#passengers" with your two columns names
- run `final.py` 
- input `streamlit run final.py` in the terminal to start the localhost 

## Future Plans  
- Add 'file upload' feature to the app so the users can directly upload their historical data 
- Add more editable parameters for the users 
- Integrate more models like LSTM


