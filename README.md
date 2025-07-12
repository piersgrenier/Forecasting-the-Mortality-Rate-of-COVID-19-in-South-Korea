### Forecasting the Mortality Rate of COVID-19 in South Korea Final Report
<br>

**Piers Grenier**
<br><br>

#### Executive summary
This project aims to answer the question of whether or not, through machine learning techniques, it is possible to forecast the mortality rate of patients living in South Korea based on their infection case, age and province of residence. The implementation of these techniques on existing COVID-19 data in South Korea must be evaluated to determine the validity of any findings. If successful, the intel drawn from these results could prove invaluable in researching new viruses and outbreak prevention. Otherwise, concerns should be raised for the potential threat of future pandemics. 
<br><br>


#### Problem Statement
Can we build a forecasting model to accurately predict the mortality rate of COVID-19 patients living in South Korea based on infection cases, age and region?
<br><br>


#### Rationale
The research question is key in recognizing seasonal trends in COVID-19 related fatalities in South Korea and using said results for informative as well as research purposes. This time series analysis may also be extended to forecast the mortality rate of similar viruses in the future, which promotes pre-emption. Consequently, failure to answer the research question not only implies an inability to accurately forecast the mortality rate of COVID-19 patients based the aforementioned factors, but also a significant vulnerability to unfamiliar viruses in South Korea.
<br><br>


#### Data Acquisition and Sources
Data consists of infection case, patient, regional and time series datasets in South Korea. The final datasets will joins these data on related attributes to forecast mortality rate of COVID-19 patients based on the nature of infection cases, age and region. 
- [Kaggle dataset](https://www.kaggle.com/datasets/kimjihoo/coronavirusdataset/data?select=Case.csv)
- [Data description](https://www.kaggle.com/code/kimjihoo/ds4c-what-is-this-dataset-detailed-description)
<br><br>


#### Methodology
(a) Preprocessing through data cleaning, feature selection and scaling

(b) Seasonal-Trend decomposition using STL, autoregressive (AR) and autoregressive moving average (ARMA) time series forcasting

(c) Gradient descent

(d) K-fold cross validation using rolling window method

(e) Graphical analysis using Matplotlib to illustrate and interpret results (**EDIT**: Seaborn and Plotly are unused)
<br><br>


#### Data Preprocessing and Preparation Steps
1. Filtered extraneous data through feature selection
2. Dropped duplicate and missing rows in initial datasets
3. Merged multiple clean datasets to acquire key features
4. Dropped duplicate and missing rows in merged datasets
5. Resolved structural errors in data (i.e. correcting data types)
6. Refined data based on target variables, number of days data is recorded, and start as well as end dates for data collection
7. Performed outlier analysis
<br><br>


#### Model Outcomes and Predictions
For this regression task:
- Unsupervised learning algorithms include: STL decomposition and gradient descent
- Supervised learning algorithms include: AR forecasting
- Other algorithms include: ARMA forecasting

Expected output:
- 
<br><br>


#### Model Selection
From the problem statement:

"""
<br>Techniques from problem statement:

(a) Preprocessing through data cleaning, feature scaling, feature selection and dimensionality reduction via PCA

(b) Time Series Decomposition and ARMA

(c) Stochastic Gradient Descent

(d) K-Fold Cross Validation

(e) Various graphical tools such as Seaborn, Matplotlib and Plotly to illustrate as well interpret results

"""

Document History:
<br>[-] Dimensionality reduction via PCA (unnecessary)
<br>[+] STL decompostion and AR models
<br>[-] Stochastic label for gradient descent (inapplicable)
<br>[+] Rolling window method for k-fold cross validation
<br>[-] Graphical tools Seaborn and Plotly (unused)
<br><br>


#### Model Evaluation
Share your model evaluation here. What types of models did you consider for your problem (classification, regression, unsupervised)?  Articulate the evaluation metrics you used and how you determined which model was most optimal for your problem.


<br><br>


#### Deployment
Now that we've settled on our models and findings, it is time to deliver the information to the client.  You should organize your work as a basic report that details your primary findings.  Keep in mind that your audience is a group of used car dealers interested in fine-tuning their inventory.
<br><br>


#### Next Steps
What suggestions do you have for next steps?
<br><br>


#### Outline of project
- [Exploratory Data Analysis](https://github.com/piersgrenier/Exploratory-Data-Analysis/blob/main/EDA.ipynb)
- [Forecasting the Mortality Rate of COVID-19 in South Korea]()

