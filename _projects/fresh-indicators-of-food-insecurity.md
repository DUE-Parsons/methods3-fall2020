---
layout: project-page
title: "FRESH Indicators of Food Insecurity"
linkname: fresh-indicators-of-food-insecurity
author: "Ashley Lehrer"
tagline: "Food Insecurity persists in NYC, FRESH policy intends to expand access to affordable healthy food retail in low income areas, has it succeeded?"
location:
    - place: New York City, NY
project-link:
    - href: https://thenewschool.carto.com/u/lehra715/builder/4601d911-e7c2-4f4e-ac7b-6ffa9b117bef/embed
tags:
    - tag: policy
    - tag:  food insecurity
    - tag:  equitable access
    - tag:  affordability
    - tag:  public health
    - tag:  zoning
thumbnail-path: img/fresh-indicators-of-food-insecurity/FJR1q5Y.jpeg
img-folder: ../../img/fresh-indicators-of-food-insecurity/
timestamp: 12/11/2020 11:36:03
---
New York City has developed multiple food related policies to address ongoing food insecurity and diet related health problems that disproportionately affect low income populations. In 2008, the Food Retail Expansion to Support Health (FRESH) program was created in response to the lack of access to supermarkets in neighborhoods across the city. To determine the highest need areas, a Supermarket Need Index (SNI) was produced through weighing multiple demographics such as: income, access to a car, supermarket to bodega ration, and rate of obesity and diabetes. These factors became a map of neighborhoods with high, medium, or low need and formed the zones that are utilized throughout the policy framework. 

NYCEDC Supermarket Need Index
![]({{ page.img-folder }}OQ7yfAg.png)

FRESH provides developers and businesses financial and zoning incentives to open food retail stores in these areas, which may otherwise be framed as too risky from an economic perspective. One particularly questionable aspect of the incentives is that developers are able to build larger residential buildings without rezoning if they commit to including a supermarket on the ground floor. Yet, there is no protection for existing residents whose properties will rise in value, potentially causing displacement and gentrification. 

FRESH Incentives
![]({{ page.img-folder }}Tzl0x7f.png)

Twelve years into this program, I wanted to analyze if the stores that have been provided FRESH incentives are actually in the areas with populations that would benefit most from increased proximity to supermarkets. Unfortunately, the SNI metric was not available to download, so I decided to utilize indicators that they had not addressed. I used American Community Survey 2018 5-year data for SNAP recipients, low income seniors, low income children, and extreme rent burden (paying over 50% of income on rent). Then I joined the data with census tract polygons, and normalized all the data to get the percentage per census tract. 

Lastly, I was not able to find a CSV of all the FRESH sites so I made my own spreadsheet by google searching the address of each site on the EDC map and geocoded the locations. For the web map, I added images of all sites and public reviews of each supermarket to get a qualitative sense of the community’s interactions with the stores.

![]({{ page.img-folder }}I4Ua5zu.png)

FRESH Zones + Sites
![]({{ page.img-folder }}sldgVUV.jpg)

From these maps, it seems as if many of the FRESH supermarkets have been located in census tracts with the lowest density of these indicators, showing that the SNI may have produced zoning areas that are too large to pinpoint the locations best suited to serve high need populations. Additionally, there are still entire FRESH Zones that have not seen any investment and others have multiple FRESH sites very close together, indicating that the zones have not been able to produce equitable distribution. 

FRESH Indicators of Food Insecurity

![]({{ page.img-folder }}4rEc3WX.png)

![]({{ page.img-folder }}CPUNJm7.png)

![]({{ page.img-folder }}qKcVRJd.png)

![]({{ page.img-folder }}xu7bA4H.png)

There are reports indicating that price, not proximity is the greatest barrier to access fresh healthy food for low income populations. FRESH stores have lessened the food deserts that characterized much of the high need areas according to the SNI, but are they actually affordable? While I was not able to address that part of the analysis for the project, I will continue to interrogate the ability for this market based approach to food security and public health to actually have a positive impact on the populations it seeks to serve. 