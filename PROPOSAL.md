- Working title: **Victoria COVID-19 Dashboard**

- Group Members
    - Atif Mahmood u4310482 u4310482@anu.edu.au (Vis)
    - Courtney Cusch u5504004 u5504004@anu.edu.au (Ana)
    - Rachael Eddowes u4270447 u4270447@anu.edu.au (Ana)
    - Shuang Sha u6922557 u6922557@anu.edu.au (Ing)
    - Jeff King u7143718 u7143718@anu.edu.au (Vis)

- Overview

    After successfully controlling the spread of COVID-19 from January to June 2020, 
    Australian governments and residents faced a much more significant second wave 
    of infections following a failure in quarantine procedure that was announced 
    publicly on May 27. This second wave of infections has disproportionately affected 
    the state of Victoria.
    
    With cases now falling, our project aims to explore a number of hypotheses about 
    the impact of demographic characteristics on the spread of COVID-19 in Victoria. 
    Specifically:
    - Do lower income areas have more cases?
    - Are areas with higher aged populations more likely to have more cases?
    - Are areas with higher education levels less affected? (Is there a difference?)
    - Are people working in particular industries more likely to be infected?
    - Is there a difference in the infection rate between the genders? What about the death rate?
    
    Our approach is to design a dashboard that will include different views, each corresponding
    to different characteristics of the population (i.e. Income, Age, Gender Education, 
    Employment, Occupation). See 'Sketch.jpg' file in our repository for an overview of the 
    basic design. While our main case study is the state of Victoria, we will perform similar 
    analyses on data depicting the COVID pandemic (in another similar state in the USA) across the USA, 
    by way of comparison. These comparisons will allow us to explore further questions such as: Is the impact of 
    sociodemographic factors such as age, gender, education, income and employment greater in the 
    American setting than in Australia?
    
    The COVID-19 cases data pack will be extracted from the official website of 'Department of 
    Health and Human Services Victoria'. The census dataset will be generated from the ABS and 
    ATO's database (see the links below or RESOURCES.md file in our repository for more details 
    on the data sources). We will adopt the postcode of different districts in Victoria as the 
    connection point for different databases. For the USA, we will source COVID case data from 
    John Hopkins, and census data from the United States Census Bureau. Finally, we will use 
    Bokeh, Geoplotlib or Dash to create data visualizations and present the results on an 
    administrative map of Victoria.
    
- Data
  - A description of where you will get your data.
    - DHHS -> https://www.dhhs.vic.gov.au/victorian-coronavirus-covid-19-data
    - DHHS -> Cases by age group and gender (downloading the tab|eau data)
    - ABS - Census 2016 DataPack
    - John Hopkins Data Set -> 
    - Bokeh -> https://bokeh.org/
    - Dash Lib -> TBD
    
- Milestones
  - Week 1 2020-09-19 - Assign roles, work out the sprints, finish data collection, preprocessing scripts
  - Week 2 2020-09-26 - Clean data, Preliminary data analysis, Write Unitest, Create a data visualization framework
  - Week 3 2020-10-03 - Complete data analysis, Finish Unitest, Continue to build data visualization models 
  - Week 4 2020-10-10 - Finish Dashboard, Finish 4-page report
 
   
- References
  - python toolbox for visualizing geographical data and making maps   https://github.com/andrea-cuttone/geoplotlib
  - Get started with Bokeh   https://github.com/bokeh/bokeh
  - COVID-19 Coronavirus Map  https://github.com/stevenliuyi/covid19
  