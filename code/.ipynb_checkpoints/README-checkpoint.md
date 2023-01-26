In the second cell, the read.excel has the path "../data/cases_2021_train_processed_2.xlsx"
As the path implies, the xlsx files are stored in a file named "data" that is in the same location as where the "code" folder will be. The read_excel file WILL NOT run unless the xlsx files are in the location mentioned above. 

The fine-tuning for XGBoost uses the gridsearch cv, hence it will take a long time to process. Hence, the fine tuning section is commented out on the code submitted as it is surrounded with """ """. If that is removed, the fine tuning will occur and will create a xgboost_tuning.txt

The same also applies to the creation and plotting of the over-fitting graph.
again, just remove the """ """ and they should work fine.




Python Version: 3.9.13 

Libraries used:

pandas
numpy
matplotlib.pyplot
seaborn
imblearn.over_sampling
sklearn.model_selection
sklearn.metrics
xgboost
