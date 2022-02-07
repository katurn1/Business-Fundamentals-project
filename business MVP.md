# Goal
Provide my client who is starting a new vinyard with a way to predict the potential quality of their wine. 

# Data
To start exploring this goal, I developed a written proposal and used data from Kaggel, 
[Prediction of quality of Wine](https://www.kaggle.com/vishalyo990/prediction-of-quality-of-wine/notebook) to do preliminary analysis. 
The dataset is related to red variants of the Portuguese "Vinho Verde" wine. 1600 rows/ 12 columns

---
- Business Problem:
How can we accuratly predict wine quality?

- Obstacle:
Client has no idea what the quality of the wine produced will be.

- Impacted parties:
Finance won’t be able to accurately  price the wine. Vineyard workers won’t know if production/ growing methods are working well nor will they know how best to improve them.

- Main Constraints:
Getting the vineyard up and running. Will take time before vines are ready for wine production unless they have been previously planted.

- Solutions:
Get accurate analysis of the wine throughout production to know potential quality, make changes to the wine if needed, and final analysis when wine is ready for aging  for final quality check.

- Impact Hypothesis :
Forecast wine quality and improve production/ growing methods.

- Technical Process:
Model will be run at each step during the wine making process once fermentation has started.

- How to Validate Approach:
Run the model on other similar wines produced in the region.

- Timeline:
Analysis and modeling will happen over the corse of the first year of production.

- Cost of Failure:
Won’t be able to accurately price the wine. Won’t be able to be fully informed when making decisions on how to improve production/ growing methods.

- Defined Success:
Wine is accurately assessed with the model.

- Benefits of Success:
Know quality of wine, accurately price wine, improve production/ growing methods for the future which will help make better quality wine.

- Defined Success:
Wine is accurately assessed with the model.

## Preliminary Analysis
For an MVP Goal I decided to provide the client with analysis of the wines in my dataset rated at a quality of 5-8. This range is where all of the good to really good wines fall.

**Findings:**

- Large majority of the wine falls well within the dry range for residual sugar (under 10), with a few outliers in the semi-dry range.
Mean- 2.45

<img width="316" alt="Screen Shot 2022-02-07 at 3 43 16 PM" src="https://user-images.githubusercontent.com/87869709/152868983-f07752ac-139f-42a7-9aef-c3d808bcbca1.png">

- 62% of wine fall within the 6.4- 8.5 fixed acidity range, median 7.9
<img width="1081" alt="Screen Shot 2022-02-07 at 3 45 56 PM" src="https://user-images.githubusercontent.com/87869709/152869279-ca86ebca-f859-4847-a032-2a2b26c4e118.png">

- Looks to a a negative relationship between Fixed Acidity and pH, the higher the pH the less fixed acidity there is.
<img width="915" alt="Screen Shot 2022-02-07 at 3 47 40 PM" src="https://user-images.githubusercontent.com/87869709/152869465-3cd83015-3fd5-4f90-adcf-29241da306c2.png">

- As quality goes up the means for Free Sulfur Dioxide and Total Sulfur Dioxide go down.
 <img width="737" alt="Screen Shot 2022-02-07 at 3 56 43 PM" src="https://user-images.githubusercontent.com/87869709/152872819-0af81c9e-2ac4-4710-b513-12e5e4779f26.png">

- The higher the the quality goes the closer the means of citric acid and volatile acidity get.
<img width="732" alt="Screen Shot 2022-02-07 at 4 11 41 PM" src="https://user-images.githubusercontent.com/87869709/152872865-9b69c978-01e2-4921-8edf-e72244d5b9b3.png">


- As quality goes up so does the mean Alcohol  % overall mean 10.42
<img width="446" alt="Screen Shot 2022-02-07 at 4 01 50 PM" src="https://user-images.githubusercontent.com/87869709/152871330-fce0e7c5-2d61-4979-974b-71ff8e1672e8.png">

- 68% of the wines fall within 0.07- 0.10 Chloride range, mean 0.087

<img width="921" alt="Screen Shot 2022-02-07 at 4 07 33 PM" src="https://user-images.githubusercontent.com/87869709/152872034-09bdafdc-41f6-415d-a879-90217d7c4409.png">


- The wines are evenly distributed across pH scale range of 2.8-4, with a mean 3.31
- A well made dry red wine typically has about 50-75 mg/L sulfites. Our Sulphates from the filtered data has a mean 0.66, well witin the trpical range.

I will use this analysis to start a draft of the slides, continue with EDA, and build a baseline model.

