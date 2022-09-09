# From Data to Model Forecast
A Sales Data Analytics from the CAMBRIDGE GARMENTS INDUSTRY


## Background:
CAMBRIDGE GARMENTS Industry (CGI) is a leading fast fashion retailer in Pakistan, that deals in traditional and western clothing styles. The company has a presence in every major city of Pakistan, operating most of the stores by itself, which goes by the name The Cambridge Shop (TCS). CGI started operations in 1970 and has seen tremendous growth due to its simple and smart Men’s fashion line-up, especially in a formal section. CGI has captured the pulse of white-collar Pakistani men, who generally like to wear quality cotton shirts, with its craftsmanship and uncompromising quality. 

## Data:
We got raw sales data for CGI Men’s shirt, which is typically used in the Supply Chain department for sales tracking and stock movement analysis. The data has multiple numerical and many categorical variables. The data is invoice influenced, where each record represents a portion of the transaction or a value of a particular shirt brand sold. To make use of this data for any Exploratory Data Analysis (EDA) and Machine Learning (ML), it is necessary to clean the data and adapt it according to our requirements. The initial dataset contains 46 columns and 670,000 records, where each record is identified by a “BillNo”. Each record contains information about the sold out shirt from TCS related to a particular “cobrand”, which results in multiple record of similar “BillNo” but of different “cobrands”.

Firstly, it is important to know how much data is available or in other words, how many missing values are in the data. Upon inspection, it is revealed that no data was missing in numeric columns, however, data that was an input from sales agents and warehouse staff has tremendous missing values. This helps us determine our way forward with data EDA and ML. To this end, we dropped a few columns with, either 100% missing data or 100% homogenous data. 

## Exploratory Data Analysis (EDA):
With clean data, we compare the location of TCS and prepare the location data of 68 positions with the help of Google Maps.  This data is further used to present locations on maps.
Furthermore, categories must speak to numerics, to this end we introduce a feature of color segmentation, which not only collects and centralize the color schemes of shirts but, helps to segments the data according to colors.
Besides, color segmentation, it is important to name variables according to the data they hold and eliminates columns with similar data. This is perhaps the most important thing when one wrangles the actual data. It includes the renaming of variables, eliminating variables, and comparing them to check whether they represent the data accordingly, through various graphs and charts.
Lastly, it is important to check the summary statistics of the data. This helps to grasp the picturewhich is represented by the numerical aspect of data. It signifies any outliers or any irregularity among numeric variables.


Before indulging in ML modeling of complex nature, it is important to know the relationship among variables in the data. As a result of this, we first normalize the numeric variables of the data. The techniques used for normalization: 
- scaling to a range(min-max)
- clipping
- log scaling
- z-score
Next, we checked the Pearson correlation and visualized it through a heat map.  This shows which variables are highly correlated and in this case, “Qty” is highly correlated with “NetAmount”, “SalesExclGST” and “GST”.

## Machine Learning:
ML has been applying in the capacity of Regression, Classification,  Clustering and Deep Learning models. “Price” has been a dependent variable in every model except Classification. “Season” is used as a output variable in Classification. The concept of taking price, is to determine the customer behaviour with regards to price. 



