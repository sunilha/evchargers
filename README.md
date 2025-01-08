### Where to set up new EV Fast Charging Station

#### Executive summary
There is significant growth in EV vehicle adaptation over the last few years. However, the 
growth of EV charging infrastructure comparatively low. EV adaption is mostly limited to pocket areas, lack of EV charging infrastructure
is one of major factor. So there is a sense of urgency to increase the 
pace of growth of EV Charging infrastructure. This opens a new avenue of business opportunities.

#### Rationale
EV Charging Stations are the fuel stations for EV Vehicles. There is a good amount of time involved in 
charging a EV vehicles. So while setting up new charging station it becomes important that we need to identify a location 
which make business sense, and it's available for wide range of users.

#### Research Question
Cluster the features which major role in identifying a good location to set up new charging station. 

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
Data Visualization:
1. Used Folium to visualize chargers, vehicles dataset on California map
2. Used t-SNE to visualize high-dimensional data in a low-dimensional space

K-means Clustering Algorithm :
1. Identified optimal number of clusters using elbow and Silhouette score method
2. Created visualization of multiple features to better understand the clustering results 

DBSCAN Clustering Algorithm :
1. Identified optimal epsilon value and number of clusters using KneeLocator from kneed library 
2. Created visualization of multiple features to better understand the clustering results

Hierarchical Clustering Algorithm :
1. Built single and complete linkage
2. Created visualization using dendrogram
3. Flatten the hierarchical cluster using fcluster

Jupyter Notebook having code for all these can be found [here](capstone.ipynb).

After above data analysis and applying clustering and hierarchical algorithms below are my recommendations.
1. There are close to 1700 zipcodes in California and EV Vehicles present in most of them, 
however it's not the same for EV Fast Charging stations i.e. only 500 zipcodes have Fast Charging station
2. There growth of EV Vehicles and EV Fast Charging Stations aren't relatively
3. Charging Stations are heavily concentrated in cities like SF Bay Area, LA, Sacramento
4. Below factors should be considered while setting new Fast Charging station
   - accessibility shopping center, restaurants 
   - median household income, total population in the zipcode

#### Next steps
1. If we can collect below data points of charging station will help in better clustering
   1. optimal distance from Freeway or high traffic street
   2. some kind of utilization/occupancy report
2. We can collect energy pricing data from all the utility service providers and model with clustering algorithms will help to come up with better recommendations

