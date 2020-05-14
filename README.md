# Avocado-Prices-Timeseries

- This analysis took a dataset on avocado prices & volumes throughout the continental US and forecasted prospective sales trends for the future. Aside from Python & Pandas, the package used for this analysis was ‘fbprophet’, an open-source forecasting tool released by facebook for timeseries forecasting

***fb Prophet:***
- Prophet is open source library released by Facebook’s Core Data Science team for python forecasting purposes.

- Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects.

- Prophet works best with time series that have strong seasonal effects and several seasons of historical data.

- For more information, please check this out: https://research.fb.com/prophet-forecasting-at-scale/ https://facebook.github.io/prophet/docs/quick_start.html#python-api

***Data Preprocessing:***
- The dataset has two categories: ‘Conventional’ , and ‘Organic’. Organic were costlier than conventional avocados which was evident uring visualising the data

- As fbprophet only accepts data presented in a specific format, data preprocessing for this project was about conforming to said format. I removed columns related to avocado purchase volumes, and stuck strictly to price and date.

*Sales Forecast for Organic Avocados: y=price per Avocado, ds=date over time*


### Predicting accuracy from original hass avocado site:

- *https://hassavocadoboard.com/category-data/?region=Total+U.S.&y=2018*

***Real data taken from Hass avocados site***
- Average -01/04 = USD 1.325
- Average -08/04 = USD 1.295

***Predicted data from forecast-1***
- Average-01/04 = USD 1.360708286
- Average -08/04 = USD 1.373267

**Accuracy in 2018 Mar 26 - Apr 8 = 95.83%**


***Real data taken from Hass avocados site***
- Average -06/05 = USD 1.22
- Average -13/05 = USD 1.265

***Predicted data from forecast-1***
- Average -06/05 = USD 1.327687
- Average -13/05 = 1.329330571

**Accuracy in 2018 Apr 30 - May 13 = 93.53%**

#### Overall Accuracy for next one month is 94.68%

***Real data taken from Hass avocados site***
- Weekly Average - 16/05/2019 = USD 1.54

***Predicted data from forecast-1***
- Weekly Average - 16/05/2019 = USD 1.0995

**Accuracy for 450th day of forecast = 71.3%**

#### The real average of USD 1.54 falls well with range of [0.514, 1.645] as predicted by model

