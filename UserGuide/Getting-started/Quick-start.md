# Quick Start

The CACI Forecaster provides planners with the best forecasting models available. These models provide superior forecasting accuracy when compared with existing workforce management products. CACI Forecaster is quick and easy to use and provides a controlled and straightforward forecast generation process.



## Creating a Forecast Model


1. Open CACI Forecaster

2. In CACI Forecaster click “New” to create a new solution

3. Type in a solution name i.e. “Forecast sunspots” in the pop-up window

4. Click “OK” to continue

5. In the “Data Importer” part of the ribbon, select the “Text” or “CSV” icon then the “Import” icon – this tells the forecaster that you are going to import a text file (the CACI Forecaster can also import from Excel files or run any process you desire using the script import to import data i.e. database extraction, data pre-processing, etc.)

6. In the pop-up window start a new importation by clicking “Next” and browse for the data file “Sunspots All”

7. After checking that the comma delimiters option is ticked, continue to click “Next” until you see the following window, below:

8. The “Sunspots All” datafile contains the target variable “Sunspots” together with lagged variables ranging from a lag of 1 to 9 years. Lagged variables can be automatically generated via an importation script if required. Select the column header “Count (year 9)”

9. While pressing shift on the keyboard select the column header “Count (year 1)”

10. Click on the “Input known” icon – these are identified as your key drivers. The columns will turn yellow

11. Select the “Sunspots” column header and click on “Target” – the column will turn pink to indicate your target

12. Now you need to select a “Start point”. Scroll down to row 200 (for example) and select the row by clicking on the row header

13. Click “Start point” – the row will turn light blue. The data above the “start point” is historic data that CACI Forecaster will use to train the model. The data below the “start point” will be used to validate the model - CACI Forecaster will only use the key driver data below the “start point” to determine the target

14. Click on the “Data Ranges” icon to set the training and forecast length parameters in the pop-up window

15. To train the forecast algorithm we are going to use data from the first row i.e. “Fixed Training Start” = 1 to the start point that we’ve set i.e. “Training to Forecast Gap” = 0. If you wish to forecast from the “Start point” to the end of the data input a large value i.e. 9999 into the “Forecast Length” field

16. Select your model from the list: Neural Networks, Regression or Decision TreeNOTE: The CACI Forecaster can invoke a batch process to run any model you desire through the “Custom Model” option.

17. Select “Train”

18. Once the model has been trained successfully, the “Forecast” icon will be enabled. Details of the model are also displayed in the output window

19. Click on the “Forecast” icon to generate a forecast. The forecast and predicted error will appear in the data table

20. Click the “Analysis” tab

21. Click on the “Line” icon. A graph of the actual target value and forecast target is displayed with a range of performance metrics

[IMAGE]


{% hint style="info" %}
 To look at comparing different forecast models or to create a forecast scenario you can keep the original model and work with a “snapshot”.
{% endhint %}

22. In the “Solution Explorer” select and right-click on the forecast file. In the pop-up menu select “Project Snapshot”

{% hint style="info" %}
NOTE: The CACI Forecaster can export data using the “External Process” option. This can be configured to create reports or to push the forecast data back into your Workforce Management tool.
{% endhint %}

23. A snapshot of the original forecast model will be created, which can be altered in the “Data” tab. You can revert back to the original forecast model by selecting the relevant file in the “Solution Explorer”

[IMAGE]