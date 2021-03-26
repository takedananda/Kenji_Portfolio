# Data Science/Analytics Project Portfolio

# [Project 1: Tokyo Apartments Analysis](https://github.com/takedananda/Tokyo-Apartments)

The aim of this project was to analyze the pricing of apartments in Tokyo. The reason why I chose to do a project on this is because my parents are living in Tokyo, and the insights I gain through this project will be useful for me in case I ever need to find an apartment to rent to go take care of them.

Rather than using a prexisting dataset, I collected the data myself by web scraping. To gather the data, I used the Selenium library on Python to web scrape the data from apartments.gaijinpot.com, which is an apartment listing website catered towards expats. Then, I went through the entire ETL process by cleaning the data using Pandas and then loaded it to a PostgreSQL database.

After the data was been cleaned, I performed exploratory data analysis on Tableau to figure out which types of information explain apartment pricing. Finally, I constructed a dashboard to condense relevant information into one visualization. The dashboard can be found here: https://public.tableau.com/profile/kenji.takeda#!/vizhome/TokyoApartments/TokyoApartmentDataDashboard

[](https://github.com/takedananda/Kenji_Portfolio/blob/main/images/monthly_rent.png)


# [Proect 2: Loan Prediction Project](https://github.com/takedananda/Loan-Prediction)

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

