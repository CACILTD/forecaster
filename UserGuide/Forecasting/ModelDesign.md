# Model Design

A number of forecasting methods are available in the CACI Forecaster.


### The Three Core Forecasting Methods
The CACI Forecaster offers three core forecasting models, each requiring input columns which are incorporated into the forecast as additional drivers. In order to allow for multiplicative data, the application provides you with the option to take the natural logarithm of the target variable prior to forecasting.  This is available in the Settings icon once you have selected the relevant forecasting method.


| Method          | Description                                                                                                                                                                                                                                                  | Input Columns                                                                                                                                        |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| Regression      | Using a stepwise approach, the application generates an equation to calculate the target variable using a linear combination of the most relevant inputs.  A multiplicative model is also possible by taking the natural logarithm of the target variable.   | Automatically selects the most relevant input columns                                                                                                |
| Decision Trees  | Classifies records into subsets of similar records (leaf nodes) by using a set of successive rules.  Once a record is assigned to a leaf node, the model’s prediction is derived using all training records from that node                                   | Automatically selects the most relevant input columns                                                                                                |
| Neural Networks | Modelled similar to how a brain works, neural networks learn how to associate inputs with the target variable.  Unlike regression and decision trees models, it is difficult to interpret the resulting model and is generally used as a black box algorithm | As this method uses all input columns, it is advisable to determine the most relevant inputs by first generating regression and decision tree models |

Table 9 Core Forecasting Methods

When including inputs, it is usually best to start with the regression model as it will select the most appropriate inputs and provide you with a visible formula (therefore giving insight into the problem).  Once you have generated a regression mode, you may find that a decision tree model shows better performance.  After filtering out any irrelevant inputs, neural networks can be used for maximum performance.  Please note, however, that neural networks require a large amount of training data.  For smaller datasets, you may find that regression performs best.


### Custom Models
In addition to the three core methods described above, CACI Forecaster offers a number of custom models that focus more on time series methods such as ARIMA and Exponential Smoothing.  Table 10 provides a description of each model and its general performance with different types of data.  More details can be found in a separate document on custom models [2].
It is worth mentioning that, apart from the ARIMA models, any input columns will be ignored.
Bespoke forecasting models can be created by CACI if required.  For more details on additional consultancy, contact CACI using the details in section 9.


_**[ Table 10 Custom Models ]**_


Table 10 Custom Models 