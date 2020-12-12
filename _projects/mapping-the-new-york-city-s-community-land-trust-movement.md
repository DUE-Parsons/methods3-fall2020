---
layout: project-page
title: "Mapping the New York City’s community land trust movement"
linkname: mapping-the-new-york-city-s-community-land-trust-movement
author: "Sara Devic"
tagline: "Visual contribution to the understanding of the housing and demographic context in which CLTs are currently emerging in New York City"
location:
    - place: New York, USA
project-link:
    - href: https://thenewschool.carto.com/u/saradevic/builder/686cc958-ac1f-48c2-a296-5d7f21c00b10/embed
tags:
    - tag: community land trusts, affordable housing, tax lien sale, displacement, collective ownership 
thumbnail-path: img/mapping-the-new-york-city-s-community-land-trust-movement/wrCEt2o.png
img-folder: ../../img/mapping-the-new-york-city-s-community-land-trust-movement/
timestamp: 12/12/2020 2:32:48
---
There is a certain momentum for the community land trust initiatives in the New York City in the recent years and especially in 2020. They emerged as a response to a housing affordability crisis by proposing a feasible, democratic, and long-lasting alternative. In my Methods 3 final project I have mapped all the existing CLTs in New York City, regardless of their property ownership status. For the location of those that are still in the organizing phase I have considered their office addresses. Given that the purpose of the project is broader understanding of the contexts in which they emerge, office addresses are still relevant because future property will most likely be in the same neighborhood. 
The goal of my project was to overlap various demographic and housing data to help reader better understand what are the characteristics of the neighborhoods in which community land trusts are emerging. The secondary goal of the project was to test the claims brought up by CLT advocates through maps and data. 

About the Model

A community land trust (CLT) is an alternative model that separates the ownership of property from the ownership of the land on which that property is built. In effect, organized citizens remove land from the private, speculative market where its value is difficult to control. Typically, CLTs are run by a board of directors whose members include three groups of stakeholders: residents or leaseholders, people who reside within its targeted community but do not live on its land, and lastly government officials, funders, housing agencies, and social service providers.


CLTs and Tax Lien Policy

One important campaign that community land trust organizers and advocates are promoting is the abolition of the tax lien policy. Namely, if your property has unpaid debt (for taxes or utilities), New York City’s Department of Finance will sell your lien debt to an authorized buyer. A lien servicing company, on behalf of the buyer, adds more fees and interest to your debt, and this process oftentimes eventually leads to foreclosure and displacement. CLT advocates are proposing that prior to any foreclosure proceeding by the City, owners could be offered to instead sell land from under their houses to a CLT. A CLT could then facilitate a mortgage refinance, and residents could stay.

In a report “Commodifying our communities: The case for abolishing NYC’s tax lien sale and prioritizing community land trusts in a new tax collection and property disposition system,” authors claim that “geography of tax lien sale properties is generally well-matched to local CLT organizations.” I have tried to test or make an evidence for this claim by overlapping data:

![]({{ page.img-folder }}S57VrU6.png)

According to the data, this year’s properties at risk of tax lien sale are almost evenly dispersed throughout the city, but locations of community land trusts are indeed in areas with a greater concentration. 

Furthermore, in the same report authors claim that low income and black and brown communities are disproportionately affected by this policy. Overlapping the city-wide data on the median household income with percentage of black and brown communities per census tract did not show such clear and bold results and lead me to think that making wide statements like that is risky. 

![]({{ page.img-folder }}tU8YKND.png)

![]({{ page.img-folder }}DwtryfS.png)

![]({{ page.img-folder }}c4MuYAB.png)

Still, certain overlaps do exist. For example, in the area around East New York in Brooklyn, in the Northern Manhattan, in the Southern Bronx and at the tip of Staten Island – the three factors do converge: the high concentration of tax lien properties, the predominance of people of color and low-income households.

![]({{ page.img-folder }}yHAWqOy.png)

![]({{ page.img-folder }}mVpqbrT.png)

Another conclusion that can be drawn from this wide perspective is the concentration of housing support programs or non-speculative housing provision models present in the lower income areas: Lower East Side, border of Brooklyn and Queens, East Harlem and South Bronx. The housing provision data I have overlapped in the online map using Carto. These are also, precisely the areas where new community land trust are emerging. 

![]({{ page.img-folder }}eQaKZQe.png)

![]({{ page.img-folder }}PpHXyuQ.png)

Data Sources
 
- CLTs in New York City: I made dataset from scratch by finding the addresses on organizations’ websites (and contacting them, if needed) and geocoded spreadsheets at Geocod.io, adding columns for Latitude and Longitude to the spreadsheet.
- Data on median income and race by census tracts are both from the American Community Survey, 5-year survey reports from 2018. These spreadsheets I have joined in QGIS with census tract attribute tables by matching their census tract labels.
- Shapefile of NYCHA developments with at least 5 residential units (700 properties with 193,445 units) I have downloaded from NYC Open data portal.
- CSV file with rent stabilized units that are deregulated since 2010 I found on the DAP portal, and then geocoded with Geocod.io. There are 8,493 properties that lost at least 20% of regulated units over the course of 10 years.
- The list of properties with tax lien sales risk in 2020 I have downloaded in separate datasets for every borough from the website of NYC Department of Finance, and then geocoded using Geocod.io.
- Dataset for existing inclusionary zoning units (158 properties with 32,044 units) I have also found at DAP portal, and then geocoded.
-  City-wide homeowners’ rate by census tract I have found on American Housing Survey in the CSV format and later joined in QGIS with census tract attribute tables by matching their census district labels (“ctlabel” column).
- CSV file on Mitchell-Lama program I have found also on the DAP portal (262 properties with 104,748 units) and then geocoded. 
- Shapefiles of NYC census tracts and borough boundaries are downloaded from NYC Open Data portal.
