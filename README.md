Executive Summary

Space travel is the future and multimillionaires are investing in it. However, rocket launches are very costly but SpaceX’s Falcon 9 rocket’s first stage is reusable and saves a significant amount of cost. In this project, I have determined whether the first stage will land successfully and gathered information relevant to the launches. Classification models were build and the best model that predicts landing outcomes were chosen.

Methodologies:

The data was collected using SpaceX’s API and Beautiful Soup HTML webpage parser. Data wrangling was done by cleaning and preparing data for model training. Exploratory data analysis was done using Seaborn to visualize data and SQL to query relevant data. Folium was used to build an interactive map to view launch sites while a dashboard was constructed with Plotly Dash. Data was trained and tested using classification models and the best model was chosen with highest prediction accuracy.
Key Takeaways:

The success rate for landing outcome is 67% with highest successful landings on drone ships at 45%. Most successful launches came from launch site KSC LC-39A and ISS seems to be the most promising orbit when it comes to launch successes with heavy payloads. Boosters like B4 and FT successfully carried heavy payloads. All launch sites are located on the coastal areas with proximities close to railways and highways but further from cities. For predictive analysis, Decision Tree model gave the highest prediction accuracy for launch outcomes at 89%.
 

Introduction

Project background and context:

Rocket launches are expensive but SpaceX’s Falcon 9 rockets can recover the first stage boosters significantly reducing launch costs. If the first stage landing outcome can be determined, the cost for each launch can be determined too. Besides that, I wanted to determine the factors that contribute to the launch successes to maximize the success rate of future launches.

Answers I needed:

1.Will the first stage be reused (successful landing outcome)?
2.Which features or factors have contributed to the successes and failures of the launches?
3.Which classification model with best accuracy can be used to predict the landing outcomes?
 
Methodology
1. Data collection methodology:

   - SpaceX API

   - BeautifulSoup HTML Parser           

2. Data wrangling

    - Data cleaning done by dealing with missing values and generating labels

3. Exploratory data analysis (EDA) using SQL and data visualization using Matplotlib and Seaborn

4. Interactive visual analytics using Folium and Plotly Dash

5. Predictive analysis with classification models using Scikit-Learn

 

Exploratory Data Analysis (Seaborn)



Flight number vs Launch Sites

There are 3 launch sites on Figure 1 and we can see that most flights are successfully launched in CCAFS SLC-40 and least launches have been done in VAFB

SLC 4E. On the contrary, CCAFS SLC-40 also has the most failed launches among the 3 launch sites.

 

 Payload vs Launch Sites

We can see on Figure 2 that both CCAFS SLC-40 and KSC LC-39A launch sites have launched rockets for massive payload mass of 16000kg. For VAFB-SLC

4E site, there are no rockets launched for heavy payload mass - greater than 10000kg.

 

Success Rate vs Orbit Types

We can infer from Figure 3 that the orbit types ES-L1, GEO, HEO and SSO have a mean success rate of 100% whereas GTO orbit has the lowest mean success

rate at 50%. Orbit SO has no mean success rate indicating that the launches are unsuccessful.

 



Figure above shows that most flight launches were done at GTO and ISS orbits whereas ES-L1, SO, HEO and GEO have one launch each. It can also be

deduced that the most flight launch failures was at GTO among all the orbits.

 



Figure shows that orbit VLEO has been used in launches with the heaviest payload mass at almost 16000kg, followed by ISS at 12000kg and PO at 10000kg.

It is notable that payload masses of 6000kg and below have been done in orbits like ES-L1, SSO, HEO and GEO and all the launches have been successful.

 



There was no success seen in launches from 2010-2013. In 2014 there was a steep increase in success rate. The success rate was the highest in year 2019

followed by 2017. In 2018 the success rate took a dip to 60%.

 

 

Exploratory Data Analysis (SQL)

 



 



 



 



 



 



 

Total Number of Successful and Failure Mission Outcomes 



 



 

2015 Drone Ship Failed Landings



 



 

 

Interactive Analytics (Folium)

 



There were 4 launch sites found on the map:

1. CCAFS LC-40

2. CCAFS SLC-40

3. KSC LC-39A

4. VAFB SLC-4E

All the launch sites were found to be on the coastal areas of US, one in the west coast (California) and three in the east coast (Florida).
 



Zoomed in map showing launch outcome markers for KSC LC-39A (13) and both CCAFS (33) launch sites.

 



Zoomed in map with launch outcome markers for both CCAFS LC-40 (26) and CCAFS SLC-40 (7) launch sites. It is noted that most launches have been done

in the east coast launch sites with CCAFS LC-40 being the highest to carry out launches (26).

 

 

 

 
