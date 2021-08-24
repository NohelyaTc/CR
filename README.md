
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

# CRT_database

La carpeta "base de datos OSRM" contiene las bases de datos con informacion de la 
estimacion del tiempo de viaje en OSRM.

data set 0 = Contiene información de los 4 meses desde enero hasta abril de 2017  (2987 SME)
data set 1 = Contiene informacion de Enero 2017
data set 2 = Contiene informacion de Febrero 2017
data set 3 = Contiene informacion de Marzo 2017
data set 4 = Contiene informacion de Abril 2017 

No UNIDAD        : es para identificar a la ambulancia que da el servicio.
DIA              : día en que se da el servicio.
MES              : mes en elque se dio el servicio.
HORA SALIDA      : hora a la que sale la ambulacia a ofrecer los primeros auxilios.
TIEMPO DE VIAJE  : tiempo de viaje por OSRM, de el punto de salida al lugar del incidente.
DISTANCIA METROS : tiempo de viaje por OSRM, de el punto de salida al lugar del incidente.
LONGITUD SALIDA  : coordenada de la salida de la ambulancia
LATITUD SALIDA   : coordenada de la salida de la ambulancia
LONGITUD LLEGADA : coordenada del lugar del incidente
LATITUD LLEGADA  : coordenada del lugar del incidente
DT               : la diferencia de tiempo de TGPS-TOSRM. (TGPS: Tiempo del GPS) (TOSRM: Tiempo de OSRM) 
SALIDA           : Etiqueta de salida DM(Decremento Medio), DP(Decremento Pequeño) y INCREMENTO.
SALIDA2          : Etiqueta de salida 3(Decremento Medio), 2(Decremento Pequeño) y  1(INCREMENTO).



