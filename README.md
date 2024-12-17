### Opportunity for EV Fast Charging Station

**Author**

#### Executive summary

#### Rationale
There is significant growth in EV vehicle adaptation over the last few years. However the 
growth of EV charging infrastructure comparatively low. EV adaption is mostly limited to cities, lack of EV charging infrastructure
is one of major factors. So there is a sense of urgency to increase the 
pace of growth of EV Charging infrastructure. This opens a new avenue of business opportunities.

#### Research Question
EV Charging Stations are the fuel stations for EV Vehicles. There is a good amount of involved in 
charging a EV vehicles. So while setting up new charging station it becomes important that we need to identify a location 
which make business sense and make sure EV infrastructure not only limited to cities. 

#### Data Sources
1. The dataset is limited to California only
2. There is partial data for the year 2024
3. EV Vehicle, Charging Station Data can be found at https://www.energy.ca.gov/
4. Demographics Data can be found at https://data.census.gov/
5. California Zipcode dataset can be found at https://gis.data.ca.gov/)

#### Methodology
Have followed CRISP-DM process which is the standard process in industry for data and machine learning projects which includes:
1. Business Understanding - Understand the problem statement
2. Data Understanding - Identify required datasets, understand the available datasets, build data definitions
3. Data Preparation - Data cleaning, drop non-significant features, encode categorical values, handling missing values, scale and normalise data
4. Modelling - Apply unsupervised clustering algorithms like K-means, DBScan. 
5. Evaluation of Results - Evaluate the quality of cluster by calculating Silhouette score, SNE and t-SNE visualization

#### Results
Data Analysis:
1. Used Folium to visualize chargers, vehicles dataset on map
K-means Clustering :
1. Identified optimal number of clusters using elbow and Silhouette score method
2. Created visualization of multiple features to better understand the clustering results 

Jupyter Notebook having code for all these can be found [here](capstone.ipynb).


After above data analysis and applying K-means clustering algorithm below are my initial findings.
1. There are close to 1700 zipcodes in California and EV Vehicles present in most of them, 
however it's not the same for EV Fast Charging stations i.e. only 500 zipcodes have Fast Charging station
2. There growth of EV Vehicles and EV Fast Charging Stations aren't relatively
3. Charging Stations are heavily concentrated in cities like SF Bay Area, LA, Sacramento
4. Below factors should be considered while setting new Fast Charging station
   - accessibility shopping center, restaurants 
   - median household income, total population in the zipcode



#### Next steps
1. Perform modelling using DBScan clustering algorithm
2. Evaluate and if application use hierarchical clustering algorithm
3. Build SNE visualization

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
