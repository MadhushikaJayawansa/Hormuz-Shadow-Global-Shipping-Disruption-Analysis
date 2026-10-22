# Hormuz-Shadow-Global-Shipping-Disruption-Analysis

## 1. Project Purpose and Motivation

The Strait of Hormuz is an important route for global shipping, especially for transporting oil and other energy resources. If access to this route is restricted due to geopolitical disruptions, ships may need to take longer alternative routes, which could increase travel time and fuel costs.

The purpose of this project is to understand how restricted access to the Strait of Hormuz could affect shipping distance, estimated travel time, and fuel costs using a simulated rerouting scenario.

To do this, I combined three Kaggle datasets covering ship movements, port activity, and fuel prices. I selected and merged the relevant columns to create a structured dataset for analysis. Using Python, I compared normal shipping conditions with a simulated disruption scenario to estimate how longer routes could affect travel time and fuel costs.



###  Objectives

- Compare shipping distance under baseline and simulated disruption scenarios.
- Estimate changes in travel time resulting from longer alternative routes.
- Quantify the estimated increase in fuel costs associated with rerouting.
- Investigate the relationship between shipping distance and estimated fuel costs.
- Apply statistical methods to evaluate differences between the scenarios.
- Visualize the conceptual route deviation and communicate its potential operational implications.


### Final Dataset

The processed dataset is available on Kaggle:

[**Download the Final Structured Dataset**](https://www.kaggle.com/datasets/madhushikajayawansha/global-shipping-disruption-hormuz-route-simulation)

This dataset serves as the analytical input for comparing baseline and simulated rerouting scenarios.


## 2. Discussion of Findings

The analysis investigates how changes in shipping routes may affect operational efficiency and fuel expenditure under the assumptions of the simulation.

### Descriptive Analysis 

#### Fuel Cost Comparison

 <img src="images/Bar plot Route_Type and Fuel_Cost.png" >

The bar chart illustrates the difference in estimated operational fuel cost between the normal shipping route (“Before”) and the disrupted rerouted scenario (“After”). The findings indicate that the disrupted scenario experienced a significantly higher fuel cost compared to the normal route.
This increase is primarily associated with the extended shipping distance caused by rerouting around Africa following the simulated disruption in the Strait of Hormuz. The results demonstrate the economic impact of geopolitical instability on maritime transportation operations and supply chain expenses. This finding supports the assumption that geopolitical disruptions can substantially increase maritime operational expenses through route deviation and extended travel distance.

### Correlation Analysis 

 <img src="images/Correlation Analysis.PNG" >

 The correlation results indicated a strong positive relationship between shipping distance and fuel cost. This suggests that vessels traveling longer rerouted distances experienced significantly higher operational fuel expenses.
The findings support the conceptual framework of the study, where geopolitical disruption leads to route deviation, increased shipping distance, and higher operational cost. Therefore, the analysis confirms that operational fuel expenditure is strongly influenced by travel distance within disrupted shipping environments.


### Hypothesis Testing

<img src ="images\Hypothesis Testing.PNG">

The T-test results produced p-values below the significance threshold of 0.05 for both fuel cost and travel time. Since the p-values were significantly lower than 0.05, the null hypothesis was rejected.
Therefore, the findings confirm that geopolitical disruption had a statistically significant impact on maritime logistics operations by increasing operational fuel cost and travel duration.

### Regression Analysis

#### Scatter plot

<img src ="images\Scatter plot.png">

The scatter plot illustrates the relationship between shipping distance and operational fuel cost. 
Each point represents an individual shipping observation. The visualization shows a clear upward trend, indicating that fuel cost increases as shipping distance increases.
A regression line was added to the scatter plot to represent the overall trend in the data. The upward slope of the regression line demonstrates a positive linear relationship between shipping distance and fuel cost.


### Geospatial Mapping Findings

<img src ="images\final Map.PNG">

Geospatial visualization was used to illustrate the difference between the normal shipping route and the disrupted rerouted path. A Folium-based map was developed to visually compare the operational changes caused by geopolitical disruption in the Strait of Hormuz.
The blue route represents the normal maritime path through the Strait of Hormuz and surrounding trade corridors. The red route represents the simulated disrupted scenario, where vessels were rerouted around the African coastline due to restricted access to the original route.

The visualization clearly demonstrates the significant increase in travel distance associated with rerouting. Compared to the normal route, the disrupted path requires a substantially longer maritime journey, resulting in increased travel time and operational fuel cost.


### Tools and Technologies

Python — analytical workflow and simulation.

Pandas — data preparation and integration.

Matplotlib — statistical and comparative visualization.

SciPy — statistical hypothesis testing.

Statsmodels — regression analysis.

Folium — geospatial mapping.

Jupyter Notebook / Google Colab — interactive analysis environment.

Kaggle — source datasets and publication of the final structured dataset.

GitHub — project documentation and version control.

<a href="Hormuz_Shadow_Global_Shipping_Disruption_Analysis.ipynb">Explore</a>
