# Forecasting

Once the user has selected a forecast model, the forecast is generated in two stages.

### Train
By selecting the Train icon in the Data – Forecasting ribbon, CACI Forecaster trains the forecast model using the training data set.  The progress of the modelling can be viewed in the Output Window, normally positioned at the bottom of the application.

Once the training is complete, the Output Window provides the user with information about the model.  For example, if running a regression model, the model equation and importance of each input variable will be listed.


### Forecast
Once the model has been trained, the user can select the Forecast icon in the Data – Forecasting ribbon.  This will populate the last two columns in the data grid: Forecast and Forecast Error.

Note that if the forecast model contains inputs, each input column needs to be populated with a forecast in order to provide a forecast for the target variable.

Progress on the forecast generation will be shown in the Output Window.  The performance of the forecast is now ready to be reviewed using the Analysis tab.
