# Data Science/Analytics Project Portfolio

# [Project 1: Tokyo Apartments Analysis](https://github.com/takedananda/Tokyo-Apartments)

The aim of this project was to analyze the pricing of apartments in Tokyo. The reason why I chose to do a project on this is because my parents are living in Tokyo, and the insights I gain through this project will be useful for me in case I ever need to find an apartment to rent to go take care of them.

Rather than using a prexisting dataset, I collected the data myself by web scraping. To gather the data, I used the Selenium library on Python to web scrape the data from apartments.gaijinpot.com, which is an apartment listing website catered towards expats. Then, I went through the entire ETL process by cleaning the data using Pandas and then loaded it to a PostgreSQL database.

After the data was been cleaned, I performed exploratory data analysis on Tableau to figure out which types of information explain apartment pricing. Finally, I constructed a dashboard to condense relevant information into one visualization. The dashboard can be found here: https://public.tableau.com/profile/kenji.takeda#!/vizhome/TokyoApartments/TokyoApartmentDataDashboard

![](/images/monthly_rent.png)


# [Project 2: Loan Prediction Project](https://github.com/takedananda/Loan-Prediction)

This project is a for a competition on the data science website AnalyticsVidhya. The goal of this project is to create a machine learning classification model that predicts whether a loan applicant shall be accepted or declined a loan, given application information.

My overall workflow was as follows:

1. Loading the data and EDA
2. Data Preprocessing
3. Model Selection
4. Data transformation & Feature Selection
5. Hyperparameter Optimization
6. Prediction Threshold Optimization
7. Model Interpretability & Uncertainty

The highlight of this project is the latter parts, in which I treated the problem as a business case rather than a data science competition. I investigated how the business can optimize profits under different pricing assumptions. I also computed metrics that will get organizational buy-ins to get the model in production.

For more information about the data, please refer to the AnalyticsVidhya site: https://datahack.analyticsvidhya.com/contest/practice-problem-loan-prediction-iii/#ProblemStatement

![](/images/Loan%20prediction.png)


# [Project 3: Time Series Analysis](https://github.com/takedananda/Time-Series---VTSAX)

This is a project for time-series analysis of the adjusted closing price of VTSAX shares. 

In this project, I first built a web scraper to collect data from Yahoo Finance website. Then, I conducted time series decomposition to gain an understanding of which type of models will be best suited for the data.

I constructed a seasonal ARIMA model that outperformed naive forecasting methods, evaluated using mean absolute percentage error. 

As a bonus learning exercise, I constructed a LSTM model to compare the classical vs the modern methods of forecasting. It turned out that the small dataset size favored the classical model greatly, which signifies the time-tested robustness of traditional forecasting approaches.

As a disclaimer, please do not modify your investment strategies according to the models created through this project. The dataset's feature space does not have the explanatory power required for reliable prediction the target variable. Profitable forecasting of stock prices is not possible with limited data. 

![](/images/Time%20series.png)


# [Project 4: Mushroom Classification](https://github.com/takedananda/Mushroom-Classification)

This is a machine learning classification project aimed to create a model that can predict whether mushrooms are edible or poisonous. The dataset was downloaded from UCI Machine Learning Repository. The dataset can be downloaded here: https://archive.ics.uci.edu/ml/datasets/mushroom

The data came with the actual values of each column being abbreviated, making it impossible to decode by itself. The dataset came with a txt file that describes what each abbreviation represent. Instead of copying and pasting those descriptions into a dictionary and mapping it to the dataframe, I emulated a real-life data extraction situation. I first imported the txt file, then used regular expressions to extract the relevant abbreviations and their actual values. I stored those information into dictionaries, and mapped them to the dataset to construct an interpretable dataset.

After the data was ready to be analyzed, I followed the traditional data science project cycle: EDA, data preprocessing, modeling, and hyperparameter tuning. 


