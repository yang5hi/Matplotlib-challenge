# Matplotlib Plots

## Background

This project is to analyze the data from a burgeoning pharmaceutical company. The company is developing potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer. The study was done on 249 mice identified with SCC tumors. A variety of drug regimen was studied over the course of 45 days, and the tumor volume in $ mm^3 $ was measured every 5 days. The drug of interest is Capomulin, among others. Python-Matplotlib is used to generate all of the tables and figures needed for the technical report of the study. The summary of the study results is shown at the end.

## DataFrame Establishment
two .csv files were used to get the full dataframe for the analysis. The data is cleaned by removing any data associated with the mouse ID that has duplicate time points.

## Statistic Analyzation Procedures

* This part shows two summary statistics tables consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

* Two bar plots were generated using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the total number of measurements taken for each treatment regimen throughout the course of the study.

* Two pie plots were generated using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the distribution of female or male mice in the study.

* The final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin were calculated and output into a DataFrame. The quartiles and IQR were calculated. **One datapoint** was quantitatively determined to be the outliers across all four treatment regimens.

* Matplotlib was used to generate a box and whisker plot of the final tumor volume for all four treatment regimens, and the outliers were highlighted with **green diamond** in the plot.

* A sample mouse that was treated with Capomulin was selected, and a line plot of tumor volume vs. time point was generated for that mouse.

* A scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen was generated.

* The correlation coefficient and linear regression model were calculated between mouse weight and average tumor volume for the Capomulin treatment. The linear regression model was plotted on top of the previous scatter plot.
