----- VERSION EN ESPAÑOL -----

Este trabajo fue realizado por [Hugo Thomas](https://perso.univ-rennes2.fr/hugo.thomas) y [Florent Demoraes](https://perso.univ-rennes2.fr/florent.demoraes) en la unidad de investigación ESO CNRS en Rennes (Francia), entre junio de 2023 y marzo de 2025. Este estudio es parte de la tesis doctoral de Hugo Thomas (Université Rennes 2, Francia / Universidad de los Andes, Colombia) así como de las actividades del [programa Modural](https://modural.hypotheses.org/le-projet-modural/el-proyecto) con recursos de la Agencial Nacional de Investigación Francesa (ANR). Los métodos desarrollados en R y aplicados a Bogotá y Lima son replicables a otras areas urbanas y encuestas de movilidad abarcando otros modos de transporte.

Este repositorio contiene scripts y datos para calcular distancias por la red vial y la red de transporte público basadas en la Encuesta Origen-Destino de Hogares de 2023 en Bogotá y la Encuesta Origen-Destino de Hogares de 2023 en Lima. El análisis utiliza bases de datos de approx. 23,000 hogares en Bogotá 6,000 hogares en Lima, 100,000 viajes en Bogotá y 32,000 viajes en Lima, así como redes vial y de transporte público bajados de OpenStreetMap u otros repositorios de datos abiertos. Los principales productos de esta sección son las bases de viajes de cada ciudad con variables adicionales indicando la distancia y las emisiones de gases de efecto invernadero (GEI) y contaminantes aéreos de cada viaje.

Los scripts hacen lo siguiente:

* Calcular la distancia de cada viaje en la base, para todos los modos existentes.
* Producir estadística básica acerca del reparto modal, la distancia de los viajes, la demanda en pasajeros-kilómetros totales (PKT) y las emisiones de GEI.
* Producir mapas originales de varios indicadores por zona de residencia: distancia por modo per capitá y emisiones de gases de efecto invernadero per capitá.

![map car-1.png](https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/map%20car-1.png)

![map ges-1.png](https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/map%20ges-1.png)

Abajo encontrará:
* El script R para [Bogotá](Distancias_EODH_2023_projection_reseau.Rmd) y [Lima](Distancias_ATU_2023_con_caminata_previa.Rmd).
* El archivo HTML para [Bogotá](https://htmlpreview.github.io/?https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/Distancias_EODH_2023_projection_reseau.html) y [Lima](https://htmlpreview.github.io/?https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/Distancias_ATU_2023_con_caminata_previa.html).

_Palabras clave:
movilidad cotidiana; encuesta de movilidad de hogares; script R; cálculo de distancia por la red vial; pasajeros-kilómetro recorridos; emisiones de GEI; emisiones de contaminantes aéreos_

----- ENGLISH VERSION -----

This work was carried out by [Hugo Thomas](https://perso.univ-rennes2.fr/hugo.thomas) and [Florent Demoraes](https://perso.univ-rennes2.fr/florent.demoraes) at the CNRS ESO research unit in Rennes (France), between June 2023 and March 2025. This study is part of a PhD thesis developed by Hugo Thomas (Université Rennes 2, France / Universidad de los Andes, Colombia) and also part of the activities of the [Modural program](https://modural.hypotheses.org/le-projet) funded by the French National Research Agency. The methods developed in R and applied to Bogotá and Lima are replicable to other urban areas and other mobility surveys using other travel modes.

This repository contains scripts and data to carry out network-based distance computation based on a Household Travel Survey conducted in 2023 in Bogotá, and a Household Travel Survey conducted in 2023 in Lima. The analysis uses databases representing approx. 23,000 households in Bogotá and 6,000 households in Lima, 100,000 trips in Bogotá and 32,000 trips in Lima, as well as road and public transport networks downloaded from OpenStreetMap or open data repositories. The main outputs of this section are the trips databases of both cities with additional variables accounting for the length, greenhouse gas (GHG) and air pollutant emissions of each trip. 

The scripts do the following:

* Computing distance for each trip on the database, for all available modes.
* Producing basic statistics about mode share, trip distance, demanda in passengers-kilometers traveled (PKT) and GHG emissions.
* Showing trip examples and discussing routing issues.

![map dist car LATS-1.png](https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/map%20dist%20car%20LATS-1.png)

![map ges LATS-1.png](https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/map%20ges%20LATS-1.png)

 Please find below:
* The R script for [Bogotá](Distancias_EODH_2023_projection_reseau.Rmd) and [Lima](Distancias_ATU_2023_con_caminata_previa.Rmd).
* The HTML rendering for [Bogotá](https://htmlpreview.github.io/?https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/Distancias_EODH_2023_projection_reseau.html) and [Lima](https://htmlpreview.github.io/?https://github.com/ESO-Rennes/Distancias_Emisiones_EODH/blob/main/Distancias_ATU_2023_con_caminata_previa.html).

_Keywords: 
daily mobility; household travel survey; R script; network routing; passengers-kilometers traveled; GHG emissions; air pollution_
