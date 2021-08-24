# CRT_database

# Abstract

This paper addresses the problem of estimating the response time to a medical emergency, specifically from the Red Cross of Tijuana (RCT), which provides most of the emergency medical services (EMS) in the city of Tijuana, Mexico.
For institutions with low funding, such as the RCT, relying on free or open source mapping systems to estimate travel times is necessary but also error prone because these systems are not tuned for ambulance movements within a city.
Therefore, this work formulates a supervised machine learning problem where the goal is to predict the difference in travel time between the ground truth travel time provided by a GPS and the approximation offered by two mapping systems, Google Maps (GM) and Open Source Routing Machine (OSRM).
To this end, this work develops a new dataset based on the EMS logs of the RCT, considering calls from January 2017 to April 2017.
The posed learning problem is solved under different scenarios, including using an off-the-shelf default configuration of a Random Forest classifier, applying a hyper-parameter optimization process and using an Auto Machine Learning (AutoML) system.
Considering all of the dataset for GM, test accuracy was 69.6\% for the first two learning approaches and 71.6\% using AutoML.
For OSRM, performance was 64.6\%, 65.2\% and 66.4\% for each of the learning approaches.
Results show that it is possible to predict the level by which a mapping system over or under estimates the true travel time of an ambulance.
Finally, the impact of the model is demonstrated by using it to solve the ambulance location problem, with notable
differences in ambulance deployments and percentage of double coverage achieved relative to using the standard mapping system. The results shows that with no correction of the travel time the percentage of double coverage is 83.90\%; on the other hand, the double coverage when using travel time correction reaches 100\%.
