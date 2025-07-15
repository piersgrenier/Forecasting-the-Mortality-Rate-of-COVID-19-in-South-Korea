<div align = "center">
  
### Forecasting the Mortality Rate of COVID-19 in South Korea: Final Report</div>

<div align = "center">Piers Grenier</div>
<br>

<div align = "center">
  
#### Executive Summary</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This project aims to answer the question of whether or not, through machine learning techniques, it is possible to forecast the mortality rate of patients living in South Korea based on their infection case, age and province of residence. The incorporation of these techniques on existing COVID-19 data in South Korea must be evaluated to determine the validity of any findings. If successful, the intel drawn from these results could prove invaluable in the research of modern viruses and preventing outbreaks. Otherwise, concerns should be raised for the threat of future pandemics. 
<br><br><br>

<div align = "center">
  
#### Problem Statement</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Can we build a machine learning model to accurately forecast the mortality rate of COVID-19 patients living in South Korea based on infection case, age and province?
<br><br><br>

<div align = "center">
  
#### Rationale</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The research question is key in recognizing fluctuations in COVID-19 related fatalities in South Korea and using said results for informative as well as research purposes. This time series analysis may also be extended to forecast the mortality rate of similar viruses in the future, which promotes pre-emption. Consequently, failure to answer the research question not only implies an inability to accurately forecast the mortality rate of COVID-19 patients based the aforementioned factors, but also a significant vulnerability to unfamiliar viruses in general.
<br><br><br>

<div align = "center">
  
#### Data Acquisition and Sources</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The data consists of a patient information dataset as well as time series datasets for different ages and provinces in South Korea. These datasets will be joined on related attributes to forecast the mortality rate of COVID-19 based on infection case, age and province data. 
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
- unsupervised learning algorithms are STL decomposition and gradient descent
- supervised learning algorithms are AR and ARMA forecasting

Expected output:
- AR and ARMA models have higher forecast accuracy for young adults as well as patients living in provinces with smaller population density
- AR and ARMA models have lower forecast accuracy for the elderly as well as patients living in provinces with larger population density
- baseline AR models experience difficulty forecasting underlying patterns in data 
- optimal ARMA models accurately forecast underlying patterns in data
- ARMA models outperform AR model on all forecasts
<br><br><br>

<div align = "center">
  
#### Model Selection</div><br>
The decision to implement the AR and ARMA models was influenced by the time-oriented arrangement of the project datasets as well as mission of building a forecasting model. Naturally, they are suitable for modeling the data at hand and approaching the research question. 

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
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In evaluating these models, both forecast the mortality rate of young to middle-aged adults more precisely than the elderly. The models also have variable accuracy in forecasting mortality rates for provinces; they perform well on provinces with high population density compared to ones with very high or relatively low population density. However, the AR models fall apart when it comes to forecasting non-linear mortality rates for which the ARMA models actually extract some underlying patterns. Comparing the Mean Absolute Errors (MAEs) reveals that, although the AR model is slightly better (lower MAE) at forecasting mortality rates based on age, the ARMA forecasts of future province data are superior. One drawback is that building the best ARMA model consumes far more time than the AR model due to grid search cross validation. Overall, the optimal ARMA model outperforms the baseline AR model in terms of detecting the trajectory of future mortality rates and yielding lower MAEs. 
<br><br><br>

<div align = "center">
  
#### Next Steps and Recommendations</div><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Finally, potential next steps to furthering research of viral outbreaks and improving the forecasting ability for COVID-19 mortality rates in South Korea include:
1. Distributing the evaluation results to identify the flaws of AR and ARMA models
2. Exploring other machine learning models for forecasting the mortality rate
3. Testing a wider range of target variables to consolidate the effects of infection cases, age and province on mortality rates
4. Considering alternative features such as the number of confirmed infections for forecasting
5. Spreading news of any breakthroughs to the general public
<br>

Some recommedations are to focus analysis on older patients who are most susceptible as well as population dense provinces where mortality rates are generally higher, implement preventative measures such as high mortality rate detection systems once models are expanded upon, and compare experimental results to ensure reproduciblity of any new discoveries. 
<br><br><br>

<div align = "center">
  
#### Outline of project</div><br>
- [Exploratory Data Analysis](https://github.com/piersgrenier/Exploratory-Data-Analysis/blob/main/EDA.ipynb)
- [Forecasting the Mortality Rate of COVID-19 in South Korea](https://github.com/piersgrenier/Forecasting-the-Mortality-Rate-of-COVID-19-in-South-Korea/blob/main/Forecasting%20the%20Mortality%20Rate%20of%20COVID-19%20in%20South%20Korea.ipynb)
<br><br><br>
