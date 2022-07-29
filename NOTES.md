**DATA SOURCES**

1. Victoria Data Source

    Our data source for Victoria includes two datasets: Australian census data and Victorian COVID-19 cases data.
    The COVID-19 cases data pack is extracted from the official website of 'Department of Health and Human Services
    Victoria': https://www.dhhs.vic.gov.au/victorian-coronavirus-covid-19-data
    The census dataset is generated from the ABS database: https://datapacks.censusdata.abs.gov.au/datapacks/

    By adopting postcode as a connection point, we combined the infection rate and case numbers from the Victoria COVID
    dataset and different social features (age,gender,education,occupation,income) from Census dataset to conduct a
    comprehensive data analysis.

2. Washington Data Source

    As above the data source for Washington includes two dataset: the US Census Bureau: https://data.census.gov/cedsci/ and
    Washington State Department of Health: https://www.doh.wa.gov/Emergencies/COVID19/DataDashboard

    By adopting county as a connection point, we combined the case numbers from the Washington Department of Health (COVID
    dataset) and different demographics (age,gender,education,occupation,income) from the US Census dataset to conduct a
    our data analysis.

    (see REPORT.md for data sources details)


**CODE OPERATION INSTRUCTION**

Our project is a comparative COVID-19 dashboard which can be divided into 5 parts: Gender, Age, Education, Occupation and
Income). The dashboard will display several plots for users to analyse and view the results.

The first part of the dashboard will show how male and female members of the population have been affected by COVID in both
Victoria and Washington with time series. The second part will give you a brief idea about how the infection rate changes
among different age groups in both Victoria and Washington. The following part will present the infection rate in different
 income groups. After that, you will see the infection rate of different educational background groups. More interestingly,
 we counted the number of total COVID cases in different occupations and produced a visualization of that at the end.

(see REPORT.md for more details)

The Bokeh Dashboard (file path: Bokeh Dashboard/Build_Dashboard.py) can be run simply by running the 
data with the relevant data sources within a python session.
The Bokeh dashboard will produce a html file as an output that can then be viewed with the relevant plots. The 
individual plots (found under Code), can be run simply by running the data with the relevant data sources within a 
python session. Each task addresses a particular analytical question.