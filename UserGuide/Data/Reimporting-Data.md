# Re-importing data

Once a forecast has been developed and the results deployed, the usual next step is to re-forecast or re-build when new data becomes available.  To do this the system has a re-import facility.  To use this option, re-press the Import button.  This will bring up the first page of the relevant Importation Wizard (Text, MS Excel or Script).
 

![Typical Import Wizard - Re-Import](imgs/Re-Import.png)


The import process will then make use of the key column.  It is assumed that the import file will be the same as the original file, that its format is the same, the column positions of each variable are the same, and that their types remain constant.  The key variable is used to overwrite any values in the data grid with values from the import data.  Therefore if you have historical data that has been changed in the CACI Forecaster but not reflected in the source data, the modified values will be overwritten with the original values.  
If Update Re-Import is selected, then any rows with key values not visible in the new source data will remain unchanged.  For example, if your import data file only contains data from March 2011, yet the data grid in the CACI Forecaster contains data from January 2011, then the updated data grid will contain data from January 2011, with the values from March 2011 taken from the new import file.  To prevent this from happening (and therefore only include the new source data in the data grid), select Clean Re-Import instead.