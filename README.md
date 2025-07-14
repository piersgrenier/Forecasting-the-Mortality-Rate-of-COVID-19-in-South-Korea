<div align = "center">
  
### Forecasting the Mortality Rate of COVID-19 in South Korea Final Report</div>

<div align = "center">Piers Grenier</div>
<br>

<div align = "center">
  
#### Executive Summary</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This project aims to answer the question of whether or not, through machine learning techniques, it is possible to forecast the mortality rate of patients living in South Korea based on their infection case, age and province of residence. The implementation of these techniques on existing COVID-19 data in South Korea must be evaluated to determine the validity of any findings. If successful, the intel drawn from these results could prove invaluable in the research of new viruses and preventing outbreaks. Otherwise, concerns should be raised for the threat of future pandemics. 
<br><br><br>

<div align = "center">
  
#### Problem Statement</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Can we build a machine learning model to accurately forecast the mortality rate of COVID-19 patients living in South Korea based on infection cases, age and province?
<br><br><br>

<div align = "center">
  
#### Rationale</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The research question is key in recognizing seasonal trends in COVID-19 related fatalities in South Korea and using said results for informative as well as research purposes. This time series analysis may also be extended to forecast the mortality rate of similar viruses in the future, which promotes pre-emption. Consequently, failure to answer the research question not only implies an inability to accurately forecast the mortality rate of COVID-19 patients based the aforementioned factors, but also a significant vulnerability to unfamiliar viruses in South Korea.
<br><br><br>

<div align = "center">
  
#### Data Acquisition and Sources</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data consists of infection case, patient, regional and time series datasets in South Korea. The final datasets will joins these data on related attributes to forecast mortality rate of COVID-19 patients based on the nature of infection cases, age and region. 
- [Kaggle dataset](https://www.kaggle.com/datasets/kimjihoo/coronavirusdataset/data?select=Case.csv)
- [Data description](https://www.kaggle.com/code/kimjihoo/ds4c-what-is-this-dataset-detailed-description)
<br><br><br>

<div align = "center">
  
#### Methodology</div><br>
(a) Preprocessing through data cleaning, feature selection and scaling

(b) Seasonal-Trend decomposition using STL, autoregressive (AR) and autoregressive moving average (ARMA) time series forecasting

(c) Gradient descent

(d) K-fold cross validation using rolling window method

(e) Graphical analysis using Matplotlib to illustrate and interpret results
<br><br><br>

<div align = "center">
  
#### Data Preprocessing and Preparation Steps</div><br>
1. Filtered extraneous data through feature selection<br>

2. Dropped duplicate and missing rows in initial datasets<br>

3. Merged multiple clean datasets to acquire key features<br>

4. Dropped duplicate and missing rows in merged datasets<br>

5. Resolved structural errors in data (i.e. correcting data types)<br>

6. Refined data based on target variables, number of days data is recorded, and start as well as end dates for data collection<br>

7. Performed outlier analysis
<br><br><br>

<div align = "center">
  
#### Model Outcomes and Predictions</div><br>
For this regression task:
- Unsupervised learning algorithms are STL decomposition and gradient descent
- Supervised learning algorithm is AR forecasting
- Other algorithm is ARMA forecasting

Expected output:
- AR and ARMA models have higher forecast accuracy for young adults as well as patients living in provinces with smaller population density
- AR and ARMA models have lower forecast accuracy for the elderly as well as patients living in provinces with larger population density
- AR model experiences difficulty forecasting underlying patterns in data 
- ARMA model accurately forecasts underlying patterns in data
- ARMA model outperforms AR model on all forecasts
<br><br><br>

<div align = "center">
  
#### Model Selection</div><br>
The decision to implement the AR and ARMA models was influenced by the time-oriented arrangement of datasets as well as mission of building a forecasting model. Naturally, they are suitable for modeling the data at hand and approaching the research question. 

<br>From the original problem statement:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"""
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Techniques:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(a) Preprocessing through data cleaning, feature scaling, feature selection and dimensionality reduction via PCA

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(b) Time Series Decomposition and ARMA

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(c) Stochastic Gradient Descent

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(d) K-Fold Cross Validation

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(e) Various graphical tools such as Seaborn, Matplotlib and Plotly to illustrate as well interpret results

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"""

Document history:
<br>[-] removed dimensionality reduction via PCA (unnecessary)
<br>[+] added STL decompostion and AR models
<br>[-] removed stochastic label for gradient descent (inapplicable)
<br>[+] added specification of rolling window method for k-fold cross validation
<br>[-] removed graphical tools Seaborn and Plotly (unused)
<br><br><br>

<div align = "center">
  
#### Model Evaluation</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Share your model evaluation here. What types of models did you consider for your problem (classification, regression, unsupervised)?  Articulate the evaluation metrics you used and how you determined which model was most optimal for your problem.
<br><br><br>

<div align = "center">
  
#### Next Steps and Recommendations</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;What suggestions do you have for next steps?
<br><br><br>

<div align = "center">
  
#### Outline of project</div><br>
- [Exploratory Data Analysis](https://github.com/piersgrenier/Exploratory-Data-Analysis/blob/main/EDA.ipynb)
- [Forecasting the Mortality Rate of COVID-19 in South Korea]()
<br><br><br>
