# Machine_Learning_Project
This is a Repo about my work in the machine learning project in the Data Science Bootcamp at The Bridge, October 2023 - May 2024

The scenario presented involves a bike rental company in a city. The problem to be addressed coexists with the need for bike maintenance. Thus, the model aims to answer how much usage load the bike system will have to be able to take out of circulation those bikes that need reviews or maintenance without affecting the service.

That is, to predict the number of people who will use the service, at what times, on which days, and which parameters influence this in order to determine the best time to withdraw the vehicles.

For this purpose, the model uses the database that can be found in one of the Kaggle competitions (accessible here: https://www.kaggle.com/competitions/bike-sharing-demand/data), about the bike service in Washington DC. Among the data are the date and time and data related to it, the weather conditions, and the number of people who used the service in each time slot. Here are the columns detailed:

datetime - hourly date + timestamp

season - 1 = spring, 2 = summer, 3 = fall, 4 = winter

holiday - whether the day is considered a holiday

workingday - whether the day is neither a weekend nor holiday

weather -

1: Clear, Few clouds, Partly cloudy, Partly cloudy

2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist

3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds

4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog

temp - temperature in Celsius

atemp - "feels like" temperature in Celsius

humidity - relative humidity

windspeed - wind speed

casual - number of non-registered user rentals initiated

registered - number of registered user rentals initiated

count - number of total rentals

The adopted solution involves converting the dates into a format that functions as columns with information such as hour, month, day of the week... instead of treating it as a time series. Subsequently, a regression model is applied to obtain the number of people who will be using the service at each moment.

---------------------

El caso que se plantea es el de una empresa de alquiler de bicicletas en una ciudad. El problema al que se quiere dar respuesta convive con la necesidad de mantenimiento de las bicicletas. Así pues, el modelo a crear pretende responder a la pregunta de cuánta carga de uso tendrá el sistema de bicicletas para poder sacar de circulación aquellas que necesiten revisiones o mantenimiento sin que esto afecte al servicio.

Es decir, predecir la cantidad de personas que usarán el servicio, a qué horas, qué días y cuáles son los parámetros que influyen en ello para así determinar el mejor momento para retirar los vehículos.

Para ello, el modelo utiliza la base de datos que podemos encontrar en una de las competiciones de Kaggle (accesible aquí: https://www.kaggle.com/competitions/bike-sharing-demand/data), sobre el servicio de bicicletas de Washington DC. Entre los datos se encuentran la fecha y hora y datos relacionados con ella, el tiempo meteorológico y la cantidad de personas que usaron el servicio en cada franja horaria. Aquí desglosadas las columnas:

datetime - fecha por hora + marca temporal

season - 1 = primavera, 2 = verano, 3 = otoño, 4 = invierno

holiday - si el día se considera un feriado

workingday - si el día no es ni fin de semana ni feriado

weather -

1: Claro, Pocas nubes, Parcialmente nublado, Parcialmente nublado

2: Niebla + Nublado, Niebla + Nubes dispersas, Niebla + Pocas nubes, Niebla

3: Nieve ligera, Lluvia ligera + Tormenta + Nubes dispersas, Lluvia ligera + Nubes dispersas

4: Lluvia intensa + Granizo + Tormenta + Niebla, Nieve + Niebla

temp - temperatura en Celsius

atemp - temperatura "sensación" en Celsius

humidity - humedad relativa

windspeed - velocidad del viento

casual - número de alquileres iniciados por usuarios no registrados

registered - número de alquileres iniciados por usuarios registrados

count - número total de alquileres

La solución adoptada pasa por convertir las fechas a un formato en el que funcionen como columnas con información tales como hora, mes, día de la semana... en lugar de tratarlo como una serie temporal. Posteriormente se aplica un modelo de regresión para obtener la cantidad de personas que estarán usando el servicio en cada momento.
