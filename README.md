# IO-ko na: Input-Output Table Analysis for Mindanao Independence
An investigation into the economic feasibility of an independent Mindanao by modeling industry interdependence and agricultural reliance using Data Science methodologies.

<img src="https://github.com/SkIym/ph-industry-interdependence/blob/main/images/SEAimg3.png" width="270" height="449">

## Project Overview
Following political discussions regarding the potential secession of Mindanao from the Philippines, this project analyzes the region's economic structure. By comparing Mindanao to the "Singapore Model"—which transitioned from a small territory to a global powerhouse—we examine if Mindanao’s agricultural wealth is sufficient to sustain a sovereign economy.

## Research Questions
* **RQ-1:** What is the predicted correlation between agriculture industry input and industry outputs of Mindanao if it chooses to separate from the Philippines, based on GDP and the input-output model of the Philippines?
* **RQ-2:** How does correlation between agriculture industry input and industry outputs of the Philippines differ across other developing countries?

##  Methodology
### Data Collection
* **Industry Use/Output:** Extracted from [ADB Data](https://data.adb.org) (2000, 2007–2022).
* **Regional GDP:** Extracted from [PSA OpenStat](https://openstat.psa.gov.ph) for Mindanao-specific data.

### Technical Workflow
1.  **Regional Estimation:** Used the **Cross-Industry Local Quotient (CLQ)** technique to estimate Mindanao's regional Input-Output (IO) table from national data.
2.  **Statistical Testing:** * Applied **Pearson Correlation** to measure industry "tightness."
    * Used **Fisher’s Method** to combine p-values for significance testing.
3.  **Machine Learning:** Developed **Linear Regression** models using dummy variables (Country/Industry) to predict future IO table trends across SEA.

## Key Results
* **Significant Interdependence:** We rejected the null hypothesis, confirming a strong correlation between agricultural inputs and industrial outputs.
* **Mindanao vs. Philippines:** Mindanao exhibits a **stronger correlation** between agricultural input and industrial output than the Philippines as a whole, indicating a highly integrated (but potentially dependent) economic structure.
* **Regional Outliers:** Indonesia's economic structure was identified as a regional outlier in the SEA context, showing different correlation patterns in manufacturing and fuel sectors compared to the Philippines.

## Discussion & Insights
The study confirms that agricultural productivity is the "engine" for Mindanao’s other industries. While this provides a strong foundation for independence (similar to Singapore's early focus on specific niches), it also highlights a vulnerability: any environmental or economic shock to the agricultural sector would have a massive ripple effect across the entire Mindanaoan economy.

## Recommendations
* **Refinement:** Incorporate interregional trade data to improve the accuracy of the estimated Mindanao IO table.
* **Analysis Expansion:** Apply **Network Analysis** (closeness and betweenness centrality) to identify which specific industries are "hubs" for the economy.
* **Sustainability:** Further research is needed to determine if a standalone Mindanao economy is sustainable in the long term without national subsidies.
