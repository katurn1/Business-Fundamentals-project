# A Window Into Quality: Using Data Science to Predict Wine Quality

## Abstract
World wide about 6.2 billion gallons of wine was drank, of that Americans hold the top spot with 872 million gallons drank in 2020. The United States wine market is anticipated to witness a Compound annual growth rate of 1.47% during the forecast period (2020 - 2025). Armed with this information the Metis family is looking to start a new winery in the USA. They plan to do something a little different, to cultivate the Sezão grape from the Vinho Verde Wine Region in Northern Portugal as their red wine varietal. This particular grape isn't grown much outside of Portugal and very little in the USA. With the Metis family being less familiar with the Sezão grape and never having grown it they are looking for a way to know the potential wine quality throughout the wine making process.

## Design
- **Business Problem**: How can we accurately forecast wine quality throughout production?

- **Impact**: Being able to accurately forecast a wines quality throughout the wine making process will lead to a better final product, enable accurate pricing of said wine, and help to improve production/ growing methods.

- **Main Constraints**: Getting the vineyard up and running. Will take time before vines are ready for wine production unless they have been previously planted. A wine lab will also be needed at the winery to test the wine samples.

- **Solutions**: Get accurate analysis of the wine throughout production and aging, run model to know potential quality, make changes to the wine if needed, and final analysis/ modeling when wine is ready for bottling.

- **Technical Process**: Model will be run at each step during the wine making process once fermentation has started.

- **How to Validate Approach**: Run the model on other similar wines produced in the region.

- **Timeline**: Analysis and modeling will happen over the course of the first year of production.

- **Defined Success**: When we take a sample of wine, using a 10 point quality scale we are able to access a minimum 5 quality wine using the model and use subsequent modeling on wine samples throughout production to help improve the quality.


## Data
The data used is from Kaggel, ["Prediction of quality of Wine"](https://www.kaggle.com/vishalyo990/prediction-of-quality-of-wine/notebook). The dataset is related to red variants of the Portuguese "Vinho Verde" wine. 

1600 rows/ 12 columns

Features used are typically tested for in wine production.

- **fixed acidity**:
most acids involved with wine or fixed or nonvolatile (do not evaporate readily)


- **volatile acidity**:
the amount of acetic acid in wine, which at too high of levels can lead to an unpleasant, vinegar taste


- **citric acid**:
found in small quantities, citric acid can add 'freshness' and flavor to wines


- **residual sugar**:
the amount of sugar remaining after fermentation stops, it's rare to find wines with less than 1 gram/liter and wines with greater than 45 grams/liter are considered sweet. Semi-dry wines may have up to 12 grams of residual sugar per liter. 

- **chlorides**:
the amount of salt in the wine

- **free sulfur dioxide**:
the free form of SO2 exists in equilibrium; it prevents microbial growth and the oxidation of wine

- **total sulfur dioxide**:
amount of free and bound forms of S02; in low concentrations, SO2 is mostly undetectable in wine, but at free SO2 concentrations over 50 ppm, SO2 becomes evident in the nose and taste of wine

- **pH**:
describes how acidic or basic a wine is on a scale from 0 (very acidic) to 14 (very basic); most wines are between 3-4 on the pH scale

- **sulphates**:
a wine additive which can contribute to sulfur dioxide gas (S02) levels, which acts as an antimicrobial and antioxidant


## Algorithms
EDA in Google Sheets

1. Upload winequality-red.csv into Google Sheets
2. Clean data
3. Filter data using quality 5-8
4. Create Mean & Mode table based on above
5. Create graphics based filtered data
6. Export unfiltered data csv to Tableau

EDA in Tableau

1. Upload winequality-red.csv into Tableau
2. Create filter using quality 5-8
3. Explore data and creat graphs to show findings


I plan to use a linear regression to look deeper into the data and confirm my findings.

## Tools
- Google Sheets for cleaning, EDA and visualization
- Tableau for visualization

## Communication
- Google Sheets to prepare, clean and analyze data are in the notebooks folder [here](https://github.com/katurn1/Business-Fundamentals-project).
- Tableau analysis and graphs [here- link 1](https://public.tableau.com/app/profile/katurn1/viz/WineQuality-Businessproject/Dashboard1) and [here- link 2](https://public.tableau.com/app/profile/katurn1/viz/WineQualityPairPlot/WineQualitypairplot).
- Presentation slides can be accessed  [here]().
- Links to files are provided [here](https://github.com/katurn1/Business-Fundamentals-project).
