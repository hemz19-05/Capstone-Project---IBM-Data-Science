🚀 Executive Summary

Space travel is the future and multimillionaires are investing in it. However, rocket launches are very costly but SpaceX’s Falcon 9 rocket’s first stage is reusable and saves a significant amount of cost. In this project, I have determined whether the first stage will land successfully and gathered information relevant to the launches. Classification models were build and the best model that predicts landing outcomes were chosen.

Methodologies:

The data was collected using SpaceX’s API and Beautiful Soup HTML webpage parser. Data wrangling was done by cleaning and preparing data for model training. Exploratory data analysis was done using Seaborn to visualize data and SQL to query relevant data. Folium was used to build an interactive map to view launch sites while a dashboard was constructed with Plotly Dash. Data was trained and tested using classification models and the best model was chosen with highest prediction accuracy.
Key Takeaways:

The success rate for landing outcome is 67% with highest successful landings on drone ships at 45%. Most successful launches came from launch site KSC LC-39A and ISS seems to be the most promising orbit when it comes to launch successes with heavy payloads. Boosters like B4 and FT successfully carried heavy payloads. All launch sites are located on the coastal areas with proximities close to railways and highways but further from cities. For predictive analysis, Decision Tree model gave the highest prediction accuracy for launch outcomes at 89%.
 

🚀 Introduction

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


🚀 Conclusions

1. The success rate for landing outcome is at 67% with highest successful booster landings on drone ships at 45%.
2. Most successful launches came from launch site KSC LC-39A with most launches done into orbits GTO and ISS, and ISS having higher mean success rate compared to GTO at 60% vs 50% respectively. 
3. Boosters like FT has successfully carried payloads within 6000kg range and B4 carried massive payloads up to 10000kg. Most launch success were seen in orbits VLEO and ISS with massive payloads (<16000kg).
4. All launch sites are located on the coastal areas with proximities close to railways and highways but further from cities. 
5. For predictive analysis, Decision Tree model gave the highest accuracy for predicting the launch outcomes for future data at 89%.


 



 



 



 



 



 



 

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

 

 

 

 
