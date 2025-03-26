# Canadian-Housing-Market-Analysis

This data set was obtained from [Kaggle](https://www.kaggle.com/datasets/jeremylarcher/canadian-house-prices-for-top-cities) and includes over 30K home listings for Canada's 45 most populous cities. The data set also pulls demographic statistics from the 2021 Canadian Census.

Pandas was used for data cleaning and preliminary EDA. Seaborn and Matplotlib were used to generate visualisations exploring distribution, correlation, and the relationship between housing price and independent variables (province, city, family income, number of bedrooms, number of bathrooms), and inform prediction models. Neither the regression or random forest models that were generated had high predictive value. Other classification models would have likely yielded similar results because this data set lacked many of the explanatory variables that are typically used to predict home prices in machine learning models (house size, local public schools, crime, back yard, garage, etc.) Moreoever, the house prices do not seem to respond in a sensible manner to some of the explanatory variables.

I ultimately found that the most remarkable story being told by this data set is the disproportionate cost of homes relative to average income, and the general unaffordability of housing across Canadian cities. So I further explored this theme with Tableau visualizations.

For the Tableau dashboard, housing affordabily was defined using the Organization for Economic Co-operation and Development's (OECD) previously published [metric](https://www.oecd.org/en/topics/sub-issues/affordable-housing.html), which defines the thresholds of affordability for price-to-income ratio (x) as follows:
- Affordable: x <=3.0
- Moderately Unaffordable: 3.0 < x <= 4.0
- Seriously Unaffordable: 4.0 < x <= 5.0
- Severely Unaffordable: 5.0 < x <= 8.9
- Impossibly Unaffordable: x > 8.9

The Tableau Dashboard can be viewed [here](https://public.tableau.com/authoring/HousingAffordabilityinCanada/HousingDashboard#1)
