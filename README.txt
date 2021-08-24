1. La carpeta "base de datos OSRM" contiene las bases de datos con informacion de la 
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



-----------------------------------------------------------------------------------------------------

1. La carpeta "base de datos Google Maps" contiene las bases de datos con informacion de la 
estimacion del tiempo de viaje de Google Maps.

data set 0 = Contiene información de los 4 meses desde enero hasta abril de 2017  (2978 SME)

Los datos estan ordenados de la misma forma que para OSRM, para este caso las columnas:
TIEMPO DE VIAJE  : es el dado por Google Maps, de el punto de salida al lugar del incidente.
DT               : la diferencia de tiempo de TGPS-TG. (TGPS: Tiempo del GPS) (TGM: Tiempo de Google Maps) 

----------------------------------------------------------------------------------------------------

Los datos usados para el algoritmo Machine Learning son: No UNIDAD, DIA, MES, HORA SALIDA,
TIEMPO DE VIAJE, LONGITUD SALIDA,LATITUD SALIDA,LONGITUD LLEGADA, LATITUD LLEGADA, SALIDA. 
