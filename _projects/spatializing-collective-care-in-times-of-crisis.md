---
layout: project-page
title: "Spatializing Collective Care in Times of Crisis"
linkname: spatializing-collective-care-in-times-of-crisis
author: "Daniela Castillo"
tagline: "This project visualizes the inequities revealed/exacerbated by the covid-19 pandemic & spatializes the collective care response across the city."
location:
    - place: New York, USA
project-link:
    - href: https://thenewschool.carto.com/u/castd986/builder/10e6fa66-bfb9-441a-9f09-b4032e3145e0/embed
    - href:  https://thenewschool.carto.com/u/castd986/builder/e5f12b08-d2ff-45d7-8750-e5c159946cba/embed?state=%7B%22map%22%3A%7B%22ne%22%3A%5B40.67553766462751%2C-73.96160982549192%5D%2C%22sw%22%3A%5B40.72271489433226%2C-73.84839914739133%5D%2C%22center%22%3A%5B40.69913045591626%2C-73.90500448644163%5D%2C%22zoom%22%3A14%7D%7D
tags:
    - tag: coronavirus
    - tag:  care
    - tag:  crisis
    - tag:  social justice
thumbnail-path: img/spatializing-collective-care-in-times-of-crisis/rkcT9tj.png
img-folder: ../../img/spatializing-collective-care-in-times-of-crisis/
timestamp: 12/11/2020 8:04:42
---
Many of the structural and specifically designed inequities that exist within our cities were further revealed to us as the COVID-19 pandemic unfolded, and continues to unfold. New York City was particularly a witness to this in the early days of the lockdown in response to the public health crisis. Now, we’ve entered a grim winter season, as Dec. 1st-4th were not just some of the deadliest days in regards to the number of daily deaths due to covid, but supposedly, in all of the history of the United States.

The NYC Department of Health has been releasing weekly data related to covid positive cases, deaths, hospitalizations, trends, etc. collected by zip code. This data has been archived [via GitHub](https://github.com/nychealth/coronavirus-data)

It was a bit tricky to dig through the website to find the most useful/usable datasets, but it was certainly a better option than scraping data from the PDF files available on the NYC Health website. With Eric’s help, I worked with a dataset that presented averages of the positive case rates on a weekly basis, and the data available at the moment went from November as far back to August. I transposed that dataset and prepared it so that it could be joined with the  zip code shapefile, and though the data was collected on a weekly basis, I averaged the weekly percentages that made up each monthly period (not all datasets started and ended directly on the first or last day of the month).

The following provide snapshots of the distribution and trends in regards to rising case rates in the city.

November
![]({{ page.img-folder }}hA8b0hR.png)

October
![]({{ page.img-folder }}hRK4bQz.png)

September
![]({{ page.img-folder }}hdOqppy.png)

August
![]({{ page.img-folder }}tDQeoSj.png)

In response to the multiple crises continuing to ravage the country (joint crises of white supremacy, police brutality, and a public health emergency), networks of mutual aid and community care have not only sprouted in a localized manner, but have truly flourished and bloomed with hundreds of city-dwellers finding ways of tapping in and providing support to neighbors. 
 
In an attempt to spatialize these networks of care, I began digging through existing datasets, as well as creating my own. Through a methodology of following mutual aid networks on social media platforms, I began saving and compiling the wide range of infographics and informational posts shared online. Since this proved to be an incredibly time-intensive tasks of compiling information on location, type, and schedule of mutual aid activities, I chose to focus on the Bushwick area specifically. (This Bushwick specific map of activities is available [on Carto](https://thenewschool.carto.com/u/castd986/builder/e5f12b08-d2ff-45d7-8750-e5c159946cba/embed?state=%7B%22map%22%3A%7B%22ne%22%3A%5B40.67553766462751%2C-73.96160982549192%5D%2C%22sw%22%3A%5B40.72271489433226%2C-73.84839914739133%5D%2C%22center%22%3A%5B40.69913045591626%2C-73.90500448644163%5D%2C%22zoom%22%3A14%7D%7D).)

In regards to the distribution of these networks overall, I turned to Mutual Aid NYC, a website that has been compiling information on resources available, for those in need or wanting to provide. Through a form embedded on the website, folks involved in mutual aid networks can submit information about the services and resources they provide, and which neighborhood areas they work within. This seemed like a great starting point, as I would not have the capacity or resources to compile this data on my own within the timespan of a semester.

I downloaded all the datasets for each of the boroughs, and began to clean up each spreadsheet so that the data could be joined on QGIS. At first, I believed I would be able to join the data utilizing zip codes, as I had for the covid-19 stats, but I soon ran into trouble when cleaning up the spreadsheets. After some troubleshooting, it became clear to me that the website had utilized Neighborhood Tabulation Areas (NTAs) as the geometries for mapping these networks (which made sense, of course, as the website had their own online interactive map)! The most time intensive aspect of the process was preparing each spreadsheet for QGIS, and I had to work borough by borough. When I joined the data to the NTA shapefiles for each borough, I made brand new shapefiles for each network, utilizing the “Dissolve” feature to combine different neighborhood tracts that each network said they serviced, revealing a layering of networks that are either 1) hyperlocal, focusing on a very particular neighborhood, or 2) far more expansive, like a coalition of networks covering a large geographic area, featuring various neighborhoods.

The process resulted in the creation of 83 shapefiles total, and the most revealing thing was noticing the areas in which there is a highest concentration of overlapping networks by playing with the opacities of the shapefiles and building them up. 

![]({{ page.img-folder }}MBF37SY.png)

In addition to mapping the distribution of these networks, I downloaded data from a resource made through Google Maps showing the location and information about free community fridges across the city. After geocoding them, the distribution in relation to historical redlining maps (with a focus on areas given the “D” grading) was quite illuminating. 

The following maps show both the fridges and mapped mutual aid networks in relation to areas given the “D” grading.

![]({{ page.img-folder }}PlZhvsJ.png)

Comparing the distribution of fridges to the areas experiencing spikes of covid cases in the present moment revealed some interesting gaps .

![]({{ page.img-folder }}435Tyhh.png)

Another goal of my mapping project was to capture the existing inequities that existed prior to the pandemic, to showcase how covid-19 disproportionately affected certain areas of the city, due to mounting precarity.

Utilizing census data from NHGIS, I mapped aspects such as allocation of health insurance, receipt of assistance from programs such as SNAP, rent burden, etc.

<img src="{{ page.img-folder }}1I6Dk6C.png" style="width: unset; max-width: 100%;" >

<img src="{{ page.img-folder }}ZIw5U9z.png" style="width: unset; max-width: 100%;" >

<img src="{{ page.img-folder }}m4dvD7H.png" style="width: unset; max-width: 100%;" >

<img src="{{ page.img-folder }}raRRbnb.png" style="width: unset; max-width: 100%;" >

Again, I took a closer look at data for the Bushwick area specifically, and I mapped the percentage of all renter-occupied units in which gross rent is 35% or more of total income, as well as recent data on evictions in the neighborhood (though a supposed moratorium is supposed to be in place.

![]({{ page.img-folder }}jjZDFny.png)

This leads to my larger questions of the relationship between these networks and larger political movements or campaigns; how does the distribution and location of these hubs of mutual aid activity relate to the dangers of eviction and displacement? How can these movements serve as capacity-building  mechanisms to strengthen self-determination and autonomy?

As a conclusion, I offer up my draft of an interactive map that shows connections between mutual aid networks and deeply rooted structural inequities. My goal is to find a way to make interactive maps that reveal these correlations for each borough. Moving forward with my research, I’m also interested in learning how community members and individuals involved in mutual aid networks define their neighborhood in regards to boundaries by sense of place over prescribed NTAs, where the peripheries of the work reaches, who comprises their neighborhood, etc.
