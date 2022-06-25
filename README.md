# Tech Startup Funding 
## Abstract
Our analysis aims to investigate the correlation between the funding stage of a tech startup (Series C or not), the GDP per capita of the country the startup is based in, and the funding amount they receive from a given investor. Our data comes from the WorldBank, a Continents CSV and a Kaggle dataset compiling startup information from TechCrunch, Crunchbase, etc. We combined the datasets to conduct a multiple regression analysis investigating the correlation between the variables listed above for tech startups in North America. This subject is fascinating because startup companies are crucial for the growth of a country’s economy. Our research could provide insightful findings that are relevant and beneficial to all of us because more startups create a healthier economy. We find that GDP per capita has a positive linear relationship with funding amounts and companies in Series C have more funding amount than the other funding stages.

## Problem Statement
As ventures, startups must gather capital to develop with their ideas. This funding comes from investors including venture capitalists, banks, hedge funds, or high net-worth individuals. The funding amount offered by an investor is based on several factors: their level of interest in the market, the company’s valuation, and what the current funding stage reveals about the startup’s growth potential. Additionally, each funding stage possesses distinct characteristics that demonstrate the company’s track record and risk, hence its Valuation score. 

![Alt text](https://github.com/Nana-322/Assessing-Impacts-of-Economic-Factors-on-Funding-for-Tech-Startups-/blob/master/Viz/venture_%24vol.jpg "Figure 1: Global venture funding across sectors for different funding stages. source: crunchbase news")

In this work, we want to assess the correlation between the funding amount (startups receive from investors) and economic variables that can reveal trends that help tech startups raise capital and boost the country’s economy. We are modeling our data with the intent to: classify, summarize patterns, and test a theory. First, we would like to classify what variables positively correlate with the funding amount that tech startups receive. Then, we will summarize our trends, and lastly, we will test the theory that Series C stage companies are more likely to receive funding from investors.

## Hypotheses
1) We expect that when the GDP per capita of the country the startup is based in increases, so does the funding amount.
2) We expect that the GDP per capita of the country the startup is based in and funding amount will increase significantly if the startup is in the Series C funding stage.

## Modeling
To test our hypotheses, we explored two main multiple regression models - a parallel slopes model and an interaction model. A backward selection approach was used in estimating models by excluding some of the 5 independent variables of interest with the aid of a VIF test to identify and avoid multicollinearity. 

## Data Sources
* [Tech Company Fundings](https://www.kaggle.com/datasets/shivamb/tech-company-fundings-2020-onwards) 
* [World Statistics Dataset](https://www.kaggle.com/datasets/mutindafestus/world-statistics-dataset-from-world-bank)
* [Continents](https://github.com/dbouquin/IS_608/blob/master/NanosatDB_munging/Countries-Continents.csv) 

## Conclusion
From our analysis, there is more evidence to support the hypothesis that there is a significant association between the positive linear relationship between the GDP per capita of the country the company is based in and the funding amount for a company regardless of whether the company is Series C or not. We find that on average,for every $1000 increase in GDP per capita, a tech startup receives a 0.5% increase in funding amount from investors, especially if they are in the Series C funding stage. Moreover, companies in the Series C funding stage receive more funding than those which are not. The models generated however don’t provide much practical significance since they explain only 14% of the variation in the funding amount received by tech companies.

![Alt text](https://github.com/Nana-322/Assessing-Impacts-of-Economic-Factors-on-Funding-for-Tech-Startups-/blob/master/Viz/fundn_amt%20%26%20gdp.png "Figure 2:"Predicted funding amounts with gdp per capita and by funding stage")

## Future Work
This research has important implications in terms of identifying what are the possible variables that might help determine the funding amount of a tech company. We have already emphasized on GDP per capita of the country the tech company is based in as well as whether the company is in Series C or not. Further research can put emphasis on which vertical (category) the tech company is in or even the region the company is based in.
