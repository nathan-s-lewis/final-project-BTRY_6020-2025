Final Project: BTRY 6020 - Spring 2025 
Instructor: Nayel Bettache 
Student: Nathan Lewis 
Cornell ID: nsl49

Overview 
A multiple linear regression model was fit to a Energy Consumption Dataset from Kaggle using Energy Consumption 
as the target variable and Square Footage, Number of Occupants, Number of Appliances, Average Temperature, 
Building Type, and Day of Week as predictor variables 
the dataset can be found here https://www.kaggle.com/datasets/govindaramsriram/energy-consumption-dataset-linear-regression?resource=download

The entire R Markdown file can be run step by step or all at once, there is a LOOCV procedure that may take a small amount of time to run on a laptop or lower end desktop
It took less than 5 seconds to run on an AMD 5800X GPU and GeForce 3080 CPU combo with 32GB of Ram 

Files 
Train Dataset (Raw File) - test_energy_data.csv
Test Dataset (Raw File) - train_energy_data.csv 
Read Me File - README.md 
R File with Document Code - nsl_49_BTRY_6020_FinalProject-2025_05_06-NSL 

Dataset Used 
Energy Consumption Dataset Linear Regression uploaded by Govidnaram Sriram 

Methods 
Histograms, box plots, summary tables, correlation plots for exploratory data analysis 
Plots of predictor variable against Energy Consumption for linearity assumption 
Pairs plots for multicollinearity assumption 
Fitted vs Residual and QQ plots for homoskedasticity and normality of residuals assumption 
Central limit theorem for normality of residuals assumption 
Forward selection 
Cross validation using K fold and LOOCV 
Manual selection of covariates 

Results
Forward selection and a CV approach lead to identical models 
These models perfectly captured the trends in the data and lead to 0 errors when using cross validation 
AIC was used to compare models within the forward selection framework 
Square footage, number of occupants, and number of appliances increased electricity consumption 
Average temperature decreased energy consumption 
Industrial > Commercial > residential in terms of energy consumption by building type 
More energy was used during the week than weekday  

Discussion 
This dataset was likely generated using a RNG and calculated the energy consumption based on the covariates, as their was no error in a CV based approach 
For this reason, it is impossible to generalize to other potential datasets 

Tools 
R Version 4.4.3 
Libraries Used - 'boot', 'corrplot' 

Contact
Nathan Lewis 
nsl49@cornell.edu
