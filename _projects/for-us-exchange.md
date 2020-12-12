---
layout: project-page
title: "FOR US EXCHANGE"
linkname: for-us-exchange
author: "MOJA ROBINSON"
tagline: "A project that maps the story of travel to formulate healing and build collectivism throughout the African diaspora."
location:
    - place: The World
project-link:
    - href: http://forus.exchange
tags:
    - tag: welcome home
    - tag:  black joy
    - tag:  black creatives
    - tag:  african diaspora
    - tag:  travel
    - tag:  heal
thumbnail-path: img/for-us-exchange/s1mrVfG.gif
img-folder: ../../img/for-us-exchange/
timestamp: 12/10/2020 15:33:13
---
Story

This project is unapologetically Black and when I say Black that includes my hood negus, sistas, africans, afro-latinos, caribbeans, the old folk, the children and most definitely the trans, queer, fem, and nonbinary community.

![]({{ page.img-folder }}jOCmjYd.jpg)

Goal

The goal of this project is to map areas where Black creatives have been, areas where Black creatives would like to go, the location of Black creatives, and the location of Black commune spaces.

![]({{ page.img-folder }}OpLDlWF.jpg)

Purpose

The purpose of this map is to encourage traveling to black people in the soon post-pandemic world. Traveling, especially back to our homeland, allows us to (1) learn who we are, (2) respect each other’s culture, (3) detangle stigmas created to further oppress us, (4) develop skills we didn't know we had, (5) to create meaningful stories and relationships, and (6) to heal. Although, traveling has alway been essential to survival and healing, it doesn't mean going far, it could simply be next door.

In addition to healing, traveling can act as an avenue to build relationships to grow entrepreneurial practices in the Black community. The fact is that in the US for every dollar of wealth a white family has, the median Black family has 8 cents, the Latino family has 10 cents, and the Asian family has 68 cents. Since the Civil War there only has been a 0.5% decrease in the wealth gap between Blacks and whites. Hence, why the Black and white wealth gap in the US has conitnued to be worse than the wealth gap in South African during Apartheid. 

It’s inherent that oppression and exploitation are still actively maintained, and ironically it’s most apparent in the Global North. I believe Black uniformity starts with entrepreneurship and with circulating dollars, which we saw a glimpse of in Tulsa during the 1920s. However, it was unfortunately burned down because it was seen by others too. Thus, I hope to create digital Tulsa(s) with this project.

![]({{ page.img-folder }}hfdUUBx.jpg)

Process

I launched this project with a Google Form asking Black creatives their mission of their art practice, if they have a passport, the countries they have traveled to, the countries they want to travel to, and their favorite place to work and/or socialize. Due to privacy and security concerns, I decided to only visualize center (centroid) points of Black creatives, which I geocoded myself. I then had to manually adjust the center point so there was no visual overlapping with different Black creatives in the same city. 

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.carto.com/u/mojarobinson/builder/84b922ee-86bc-487c-92b2-65dbd6ce065c/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

Secondly, I mapped three supporting maps. The first being, the tourist average daily cost of living per country. Where I used World Data and Country specific census information to get the monthly average cost of living per country (Z). Then I surveyed a focus group, asking them on average how much more they spend when they travel. Subsequently, I worked with a travel planner to average out my findings, which led to the assumption that people spend 65% more when traveling. Where I then solved for tourist average daily cost of living per country (X) with the following equation: X = [ ( Z / 30 ) * .65 ] + Z

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.carto.com/u/mojarobinson/builder/a4c532a7-c1fc-4e75-bb02-f96e8c0098e8/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

Moreover, I used US census data to visualize metropolitan areas that are within areas where Black population is 10.7% or higher. I specifically chose 10.7% to highlight Dr. Claud Anderson’s Black population to white uncomfortability index and averaged it with the current US Black population. 

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.carto.com/u/mojarobinson/builder/7a9e3ced-7c10-40bf-ac94-81f22cfeffe2/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

Lastly, using the UN’s world tourism data and the qGIS buffering tool, I projected US National Parks that are within 60 miles of areas where Black population is 10.7% or higher. As exposure to nature not only makes you feel better emotionally, it contributes to your physical wellbeing, reducing blood pressure, heart rate, muscle tension, and the production of stress hormones.<sup>2</sup>

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.carto.com/u/mojarobinson/builder/5097f2a2-1266-4351-82fa-211f8b546f24/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

As this is an extensive ongoing project, I’ve created a geoweb portal; as participants fill out the Google Form, they instantly get added to the map via Carto Google Sheets auto-update function. Lastly, to make this project easily shareable for social media, I have continued to create themed stagnant maps using various qGIS features such as heat mapping, the OpenLayers Plugin, and a heap of vectoring tools.  

![]({{ page.img-folder }}SJBTHD6.jpg)



With Gratitude,

Moja 


Notes

1. Moja Robinson, “PANTONE®, A SOLO EXHIBITION” [https://mojarobinson.com/art](https://mojarobinson.com/art). 2019
2. “How Does Nature Impact Our Wellbeing?” Taking Charge of Your Health & Wellbeing, [takingcharge.csh.umn.edu/how-does-nature-impact-our-wellbeing](http://www.takingcharge.csh.umn.edu/how-does-nature-impact-our-wellbeing). 
