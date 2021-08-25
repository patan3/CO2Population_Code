# CO2 Emissions & Population Growth Analysis - Code

The aim of this study is to analyze the relation between the CO2 emission and the population growth of a given country. 
The interest is on whether there is a link between them and how it changes over time and among different parts of the world.

This study consists of three parts and one web application. The three notebooks can be run in any prefered order. 

## '0_Data_Import_Cleaning.ipynb'
The data is retrieved from two different sources: the first one is ['CO2 Emission From Fuel Combustion 2020 Edition'](https://iea.blob.core.windows.net/assets/474cf91a-636b-4fde-b416-56064e0c7042/WorldCO2_Documentation.pdf), from the International Energy Agency. The dataset consists of multiple sheets. 'KAYA' is the one of interest in this work. It covers a period that goes from 1971 to 2018. For a given country or region, it gives information about five different indicators. The two indicators taken into account in this study are 'CO2 Emissions' and 'Population'. Both of them are indices: the first one represents the CO2 fuel combustion emissions, while the second one identifies the population. The reference value is 100. The reference year is 1990 for all the countries, aside from some exceptions that can be found in the documentation. The second one is ['The World Bank'](https://data.worldbank.org/indicator/SP.POP.GROW), after filtering with the 'Population growth (annual \%)' indicator. The dataset gives information on the annual population growth for a given country from 1960 to 2020.
The two datasets are then cleaned and processed so that it is possible to use them appropriately. Moreover, for the final part of the analysis, the two datasets are merged so that the CO2 index and the annual population growth can be studied jointly.

## '1_Exploratory_Data_Analysis.ipynb'
Exploratory data analysis that aims to answer some of the research questions by providing interactive visual insights. In particular, the CO2 emissions index, the population index, and the annual population growth indicator are studied over the considered period (1971-2018) and over several regions, continents and countries.

## '2_Data_Modelling.ipynb'
The association between the annual population growth variable and the CO2 emissions index is studied quantitatively with the Pearson Correlation Coefficient. Additionally, for identifying countries that are more similar to other countries with respect to the others based on the aforementioned variables, a cluster analysis is performed.

## Dashboard
In order to give to the reader an overall tool for playing interactively with the several graphs and parameters, a dashboard is created. [Reach the application here](https://share.streamlit.io/patan3/co2population/Dashboard.py).
