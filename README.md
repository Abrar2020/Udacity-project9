# Udacity-project9
The Codes is divided into three parts 
This first one is for data preprocessing and Explority data analysis: 
src_Visualization _Suicides_Rates-Regression_chapter3.ipynb

Reading the row data, I uploaded data in Git-hub : 
master.csv
Countrey-Region.xlsx
WDIEXCEL.xlsx (is very common dataset) 

The missing values in row data in two features:   HDI and unemployment rates 
The first one by mean of HDI in each country , else by 0 
df['HDI_for_year'] = df.HDI_for_year.fillna(df.groupby(["country"])["HDI_for_year"].transform(np.mean))
and the second one is 
according the country code fetching unemployment index and imputing in unemployment index 
by the mean of the each country 
as df['unemployment index']=df['unemployment index'].fillna(df.merge(df_tempo,on='country',how='left')['unemployment index_y'])
until line 33 is the finish step , there is no missing values 

then Add more visualization and more relations between features  After That , there is use the data after clean and prepared for the Models 
Regression_LR-OLS-SVR-RFR-XGBR_ALL_countries
More Detailed info 
GradientBoostingRegressor  

Thank you for support and understanding 


