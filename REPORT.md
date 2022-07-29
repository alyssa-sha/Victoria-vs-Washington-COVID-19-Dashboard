# COVID-19 Dashboard – Comparing rates of infection across the populations of Victoria, Australia and Washington state, USA

## Background to the problem

After successfully controlling the spread of COVID-19 from January to
June 2020, Australian governments and residents faced a much more
significant second wave of infections following a failure in quarantine
procedure that was announced publicly on May 27. This second wave of
infections has disproportionately affected the state of Victoria. With
cases now falling, our project aims to explore a number of hypotheses
about the impact of demographic characteristics on the spread of
COVID-19 in Victoria. Specifically:
* Do lower income areas have more cases?
* Are areas with higher aged populations more likely to have more cases?
* Are people with higher education levels less affected? (Is there a difference?)
* Are people working in particular occupations more likely to be infected?
* Is there a difference in the infection rate between the genders?

Using open-source demographic and COVID case data, we have designed a
dashboard that includes different views, each corresponding to different
characteristics of the population, specifically: Age, Gender, Income,
Education, and Occupation. While our main case study is the state of
Victoria, we have performed similar analyses on data depicting the COVID
pandemic in Washington state, USA, by way of comparison. Washington was
chosen for its similar demographic profile to Victoria.Introducing
Washington database to conduct statistical analysis under the same
subject can make our results more reliable and more general. Also, these
comparisons have allowed us to explore further questions such as: Is the
impact of sociodemographic factors such as age, gender, education,
income and employment greater in the American setting than in Australia?

## Scope and limitations of the study

This study was limited by the time allocated (4 weeks), and the scope of
the course, which focused on data analysis and visualisation techniques
using Python, but did not include any statistical analysis. As such, our
findings are general in nature and have not undergone rigorous
statistical interrogation.

### Limitations of the data

Large-scale social research, and particularly censuses, is costly and
time-consuming to undertake. As a result, while population-level
demographic data is publicly available, it is not regularly updated. In
the USA, a population-wide census is conducted every ten years, with
estimates projected for the intervening years. Unfortunately for this
study, the next American census is open now, meaning the data used was
based on projections that are now ten years old. In addition, survey
participation is not comprehensive, meaning data was not available for
all counties in Washington state across all demographic variables in the
study; in particular, income data was only available for 20 counties. Likewise, census data for the state of
Victoria, Australia was limited by the interval of data collection;
censuses are conducted every five years in Australia.

## Data sources and analysis

**Income**: "Total household income (Weekly) by household composition"
from 2016 Census DataPack for Victoria by postal area
https://datapacks.censusdata.abs.gov.au/datapacks/ "Income in the past
12 months (in 2019 inflation-adjusted dollars), 2019" from US Census
Bureau:
https://data.census.gov/cedsci/table?q=s1901&t=Income%20%28Households,%20Families,%20Individuals%29&g=0400000US53.050000&tid=ACSST1Y2019.S1901&hidePreview=false

**Education**:
"2016Census_G40_VIC_POA" from 2016 Census DataPack for Victoria by postal area 
https://datapacks.censusdata.abs.gov.au/datapacks/
"Washingtion_Education_data_with_overlays_2020-10-05T043218" from US Census Bureau: 
https://data.census.gov/cedsci/table?t=Educational%20Attainment&g=0400000US53&y=2019&d=ACS%201-Year%20Estimates%20Detailed%20Tables&tid=ACSDT1Y2019.B06009

**Age Group**
"Median age" for each postal area of Victoria is from 2016 Census DataPack: 
https://datapacks.censusdata.abs.gov.au/datapacks/
"Age group and Sex" data for Washington is from US Census Bureau: 
https://data.census.gov/cedsci/table?q=ACSST1Y2019.S0101&tid=ACSST1Y2019.S0101&hidePreview=false
"Age group" data for Victoria is from 2016 Census DataPack: https://datapacks.censusdata.abs.gov.au/datapacks/

**Occupation**:
"Occupation by Age by Sex", from 2016 Census DataPack for Victoria by postal area
https://datapacks.censusdata.abs.gov.au/datapacks/

**Gender**
Washington, USA gender  data was taken from GenderSci lab's COVID-19 'US Gender/Sex COVID-19 Data Tables.
https://www.genderscilab.org/gender-and-sex-in-covid19/#CaseDeathbySex

Victoria, Australia gender data taken from the VIC Department of Health and Human Services Victorian coronavirus (COVID-19) data
https://www.dhhs.vic.gov.au/victorian-coronavirus-covid-19-data

**COVID-19 Cases**: "Victorian active cases by postcode" from
https://www.dhhs.vic.gov.au/victorian-coronavirus-covid-19-data "Cases
and Deaths by Week of Illness Onset, County, and Age" from Washington
State Department of Health:
https://www.doh.wa.gov/Emergencies/COVID19/DataDashboard#downloads

**Data linkages**: In the Victorian datasets, COVID cases and demographic
variables were linked by postcode. In Washington, the linkage was by
county.

## Findings

### Age

Across both Victoria and Washington, COVID-19 infection rate peaked
amongst young adults. In Victoria, the infection rate was 0.466% in the
20-29 age group, while it was 1.73% for people aged 20-39 in Washington
state. There could be a number of reasons for this: young people may be
working in less stable employment, and perhaps have fewer options to
work from home or take sick leave; younger people may have more active
social lives, and be more resistant to social restrictions; and people
in this age group are more likely to have small children, who are harder
to teach good hygiene habits.

Besides, the infection rate is relatively higher among the people over
80 years old both in Victoria and Washington. In Victoria, 80-89 is the
age group with the highest infection rate. 80-89 is the age group with
the second highest infection rate in Washington. We can see from the
results that no matter in Australia or in USA,People aged 70 years and
over are at greater risk of getting infected by corona virus. The
possible reason is that as people age, their immune system weakens,
which makes old people more vulnerable to infections of virus. Based on
the medical research, when the immune system gears up in older people,
there is also a higher likelihood of a phenomenon called a cytokine
storm. This is where the immune system overreacts and produces too many
of the chemicals to fight an infection.

In addition, we explored further about the infection rates in different
age regions of Victoria and tried to answer "Are areas with higher aged
populations in Victoria more likely to have higher infection rate? We
adopted the postcode to combine infection rate of the district and its
median age level. Although the trend is not that clear, we can still
find that for the areas with median age around 20 and 70, the infection
rates are slightly higher. The statistical results and reasons behind
are sort of consistent with the studies above.

### Gender

There is a small but consistent difference in the way male and female
members of the population have been affected by COVID in both Victoria
and Washington, with more female cases on average in both states. In particular, during peak infection periods,
women were infected more often than men. This could
be due to more women being in frontline and caring roles, and therefore
experiencing more occupational exposure, or physiological reasons which
are beyond the scope of this study.

### Income
In Victoria, median household income in each postcode did not seem to
have an effect on the rate of infection with COVID-19. In Washington
state, infection rates were much higher, with a mean infection rate
across all counties of 0.125 cases per capita (mean infection rate in Victoria = 0.0035). There
appears to be a skew towards counties with lower median incomes, however
the data is limited, as described above under *Limitations of the data*.

### Education
In Victoria, Australia there wasn't much of difference between education 
levels and infection rate. However, Washington, USA had a seemingly 
large difference between "Other" and the rest of the higher education levels. 
There is also a presumably large difference between Washington and Victoria, 
which could be explained by the larger population in Washington when compared 
to Victoria and also the differences in success with controlling the spread 
between the two countries. Unfortunately, due to the limitations of the 
analysis, outlined in *limitations of the data*, it is difficult to infer 
anything.

### Occupation

THe occupation task looked at the number of cases across different occupation categories
provided to us through our dataset. THe idea behind this was to assess if there are any particular
occupations that might be more at risk of being infected, and therefore propose policy that might
address this. Overall in our results professionals seemed to have the highest proportion of COVID cases
when compared other occupations. A limitation of this data is, most jobs can be deemed to be professional 
jobs so the results are not indicative of any specific systematic issues that can be highlighted. THe proportion
overall across different sectors was about the same (10%), which means the virus is somewhat evenly being
spread through the community.

## Future directions
As COVID-19 continues to spread around the world, with many countries 
now experiencing a “second wave”, there is continued interest in 
understanding this pandemic and how it affects populations of all sizes.


While this study was limited in scope, it highlights some interesting trends
in COVID-19 infections in Australia and the USA, specifically that age groups 
are differentially affected, and that more women than men seem to be infected 
during peak infection periods. Once the 2020 Census data is released, it will be
informative to delve deeper into the patterns of infection across different 
income brackets in the population. Our visualizations can help governments
and other institutions understand what social prospects to work on in order to
avoid any similar pandemics. Besides, our dashboard can help users understand
the development characteristics of the epidemic and support related in-depth research.

