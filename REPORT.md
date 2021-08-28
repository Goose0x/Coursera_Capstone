<h3> Coursera Capstone Project: Week 5 </h3>
<p align="center"> <h2> Project Title: "The New Silicon Valley: Why Miami is the New Hotspot for Tech Innovation." </h2> </p>
<h4> By: Goose0x </p> Date: August 28 2021 </h4> <p>

<b>1.0 Introduction </b><p>
<b>1.1 Background </b><p>


The results of the COVID-19 pandemic have put a major strain on businesses due to government policies, paired with a rising income tax rate, and high cost-of-living.  As a result many businesses are looking for alternative places to setup, or move to.  This year we are seeing that many major key players in the tech industry are looking for alternative locations and local governments who support entrepreneurs and businesses to support the goals of the company. <p>
This is a major shift again in history (like the gold rush in the mid 1800's, and Silicon Valley in the early 1900s to today) now seeking less government restriction elsewhere for booming technical innovation, lower crime rate, and better living conditions.  Which could also bring in more people and money to the cities. <p>
For the Capstone Project I will be investigating why tech businesses are choosing to move to Miami versus staying in Silicon Valley, San Francisco Bay, CA. and Why places like Miami, FL and Austin, TX are so attractive? <p>

<b>1.2 Problem </b><p>
 
This poses a unique situation for California, adapt or lose business.  The data collected will be the average cost of living for each location, income tax and other tax for each area. <p>
Average cost of labor, and business related incentives that make comparisons of the two states.  The report will also discuss the crime rate statistics, environmental factors and attractions <p> 
to include local restaurants, housing areas, etc using FourSquare API data.<p>
  
<b> 1.3 Interest </b><p>
This information, compiled into a report would be beneficial for businesses looking to expand or move to alternative locations in order to maintain business in the United States and avoid
high taxes, overcrowded cities and are places their business and families can grow.
  
<b>2.0 Data Acquisition and Cleaning </b><p>

<b>2.1 Data Sources </b><p>

Data for comparison was collected from a variety of sources.  At some locations it was able to be utilized as is.  For others, it would require further analysis and cleansing. <p>
The zipcodes geodata for [California GeoData](<https://www.geonames.org/postalcode-search.html?q=california&country=US>) and for [Florida GeoData](<https://www.geonames.org/postalcode-search.html?q=florida&country=US>). <p>
Cost of living data was collected here [Cost of Living Comparison](<https://www.bestplaces.net/cost-of-living/santa-clara-ca/miami-fl/250000>). <p>
Income Taxes and Other Taxes for [California Income Tax](<https://smartasset.com/taxes/california-tax-calculator>)and for [Florida Income Tax](<https://smartasset.com/taxes/florida-tax-calculator>). <p>
Occupational and Labor Statistics were downloaded from here [California Labor](<https://www.bls.gov/oes/current/oes_ca.htm#15-0000>) and for [Florida Labor](<https://www.bls.gov/oes/current/oes_fl.htm#15-0000>). <p> 
Business Incentives for comparing the states were from here [California Business](<http://apps.csg.org/BusinessIncentives/StateProfile.aspx?id=5>) and for [Florida Business](<http://apps.csg.org/BusinessIncentives/StateProfile.aspx?id=9>). <p>
Crime statistics for each state were collected from here [Santa Clara County, CA](<https://www.santaclaraca.gov/our-city/departments-g-z/police-department/crime>) and from [Miami-Dade County, FL](<https://www.miamidade.gov/global/police/crime-statistics.page>). <p>
  
 <b>2.2 Data Cleaning </b><p>
  
 The geolocation data was webscraped using beautiful soup and was exported as a txt file.  The file was then compiled and cleaned utilizing IBM Watson Studios.
 Compiled into this [CSV](<https://github.com/Goose0x/Coursera_Capstone/blob/master/CSV/zip_codes_cal_fl.csv>).<p>
 Initial issues with the data collection posed problems, as locating sufficient data, cleaning it, and getting the values to correctly display posed a problem when utilizing GeoLocator with Python.  Once the data had been collected, and properly formatted into a text file.<p> 
 The tools provided within IBM Watson Studios made the task of cleaning, organizing, removing, and sorting easy.  
 Once the data was imported, a flow was created to <i> Filter </i> only "Santa Clara" + "Miami-Dade". <p>
 The data then was verified and "Na" values were present in the data set under "Latitude" and "Longitude".  This was cleaned with a <i> Remove </i> operation.
 The data was verified again for any "Na" values using .isnull. <p>
 The dataset was then imported into the Jupyter notebook as part of the Data section, which lists the zipcodes and geo data for Santa Clara County, CA and Miami-Dade County, FL. The dataset was further broken into two dataframes, Santa Clara and Miami. <p>
 This dataset was used for FourSquare's API to review local data in the Miami, FL vicinity. <p>
 
 <b>3.0 Exploratory Data Analysis </b><p>
 
 
 
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

![California Tax Breakdown](https://github.com/Goose0x/Coursera_Capstone/blob/master/Images/CA_Tax.PNG "California Tax Breakdown").
