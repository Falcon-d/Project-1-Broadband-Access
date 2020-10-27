# Broadband-Access
An analysis of census demographics data vs broadband access in 2017.

## Table of Contents
* [General Info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Conclusion](#conclusion)
* [Sources](#sources)

## General Info
Broadband access is quickly becoming a necessity in the modern world, especially as working from home is encouraged (if not mandated) in the wake of the novel
coronavirus.  As technology becomes increasingly important in our lives, the ability to access that technology may become a barrier to improving the lives of oneself,
and one's family.  In the worst case, it may even happen that some Americans, unable to access broadband internet, lose working and educational opportunities, further
perpetuating cycles of poverty. As industry is also a possible reason why communities may have specific resources, we were also concerned with the impact of industries
on broadband access. With this in mind, we ran linear analyses on a number of census datasets against broadband access as a percent of the population at county level.
The census data came from the ACS5 survey (racial, income, age, poverty, population), and the economy-wide key statistics survey, both from 2017.  The broadband access
data came from an ASU data portal.

This project was done for a data visualization bootcamp with particular interest towards learning to use both the url and the python module to access the census API.

## Technologies
* Python version: 3.6.10.final.0
* Pandas version: 1.0.4
* Numpy version: 1.18.1
* Matplotlib version: 3.2.1
* Scipy version: 1.4.1
* Census python module

## Setup
In order to rerun these programs, a config.py containing an API key for the census API (named "census_api_key" as a string) and located in 
the notebooks folder will be necessary.

## Conclusion
In spite of the sheer volume of possible relationships examined none correlated well with broadband access. The largest r-squared value was .145 for population,
indicating that, on a county level, there is no meaningful correlation between broadband access and any racial data, income level, median age, population count,
or workers in various industries. While disappointing for someone attempting to figure out why broadband access is where it is, this is strongly encouraging for those
interested in ensuring access to techologies necessary for living in the modern world. Further research into the topic may benefit from running a time series analysis
(almost all of our analyses were set in 2017,  with the process of running a time series just starting), or by further "zooming in" on geographical location. However,
as the broadband data was accessed on a county level, the present broadband data would be insufficient.

## Sources
https://www.census.gov/data/developers/data-sets/economic-census/2017.html  
https://www.census.gov/data/developers/data-sets/acs-5year/2017.html  
https://techdatasociety.asu.edu/broadband-data-portal/dataaccess/countydata  
