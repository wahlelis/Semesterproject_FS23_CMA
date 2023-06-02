# Proposal for Semester Project

**Patterns & Trends in Environmental Data / Computational Movement Analysis Geo 880**

| Semester:      | FS23                                     |
|:---------------|:-----------------------------------------|
| **Data:**      | Movement data from lisa / the class pool |
| **Title:**     | Detecting mountainbikers                 |
| **Student 1:** | Aurelia Möri                             |
| **Student 2:** | Lisa Wahlen                              |

## Abstract

<!-- (50-60 words) -->

Mountainbiking is a sport which becomes more and more popular in Switzerland. It is therefore interesting, to assess the behavior and pattern of mountainbikers. This information can not only serve community planning, but also be out of interest for the support of legalization of trails in Switzerland.

Deriving information about where and when people ride mountainbikes can be extracted out of mountainbiking directed apps such as trailforks or strava. But filtering general movement data for mountainbiking patterns could provide more information also about illegal trail uses.

## Research Questions

<!-- (50-60 words) -->

Following this thought, we developped the research questions following below:

-   How can we detect moutainbikers, meaning all bikers riding downhill using gravity offroad?

-   How can we tell mountainbike trajectories from other movement data? (detect movement patterns of mountain bikes) 

-   How do sinuosity and turning angle influence the speed of bikers? 

-   Can we detect a similar connection between sinuosity and speed in bike trajectories in urban areas? Or in other words: how mucht do stops and red lights slow us down? 

-   Can the speed be linked to the steepness/narrowness of the curves encountered on the trail? 

## Results / products

<!-- What do you expect, anticipate? -->

We expect to find multiple sets of mountain biking patterns which could also be used for further evaluation. Furthermore, we expect that the turning angle generally decreases the speed of the bikers. The amount of curves (sinuosity) in a mountain bike descent decreases the average speed of the trajectory. We expect that the same happens to cycling movement data in urban areas, probably even more so due to red lights and crossroads.  

## Data

<!-- What data will you use? Will you require additional context data? Where do you get this data from? Do you already have all the data? -->

To characterise the moving pattern of mountainbiking we will use Lisa's recorded data with the posmo app. To compare it with other moving patterns we might use data from the data pool of our class.  

To detect which are the mountainbike trajectories, we might need a map of some mountainbike trails or a basemap to localize likely mountainbike paths? E.g. movement data within a city might not be part of a mountainbike trail, we assume that mountainbike trails are localised in steep and rural environments.

For ground truthing the mountainbike trajectories, we might need a map of some mountainbike trails or a basemap to localize likely mountainbike paths. E.g. movement data within a city might not be part of a mountainbike trail, we assume that mountainbike trails are localised in steep and rural environments. This could be an alternative to the detection based on moving patterns. 

## Analytical concepts

<!-- Which analytical concepts will you use? What conceptual movement spaces and respective modelling approaches of trajectories will you be using? What additional spatial analysis methods will you be using? -->

**Trajectory segmentation** to separate the downhill parts of the mountainbike trails. We will do this probably by excluding movement data below a certain speed threshold. 

**Speed** ,We will measure the average speed of a downhill segment. (or the speed before and after a curve on the trail, depending on the segmentation). 

**Sinuosity** and/or **turning angle** and how they influence the mountainbikers on different trajectories. (Laube & Purves, 2011) 

Movement patterns for mountainbike detection? 

-   Repetition (revisiting the same route) 

-   Slow uphill, fast downhill. Speed difference 

-   Rural/natural environment, hills. Topographical context. 

other criteria to be assessed. 

Laube, P. & Purves, R. S. (2011). How fast is a cow? Cross-Scale Analysis of Movement Data. Transactions in GIS, 15(3): 401--418 

## R concepts

<!-- Which R concepts, functions, packages will you mainly use. What additional spatial analysis methods will you be using? -->

preprocessing tools (readr, dplyr)

We will use R packages from the tidyverse for data wrangling and tidying. Exploratory data analysis and visualisations can be executed with ggplot2. For spatial data we expect to use the packages sf, tmap, For spatial data we expect to use the packages sf, and for visualisations tmap or leaflet might come into play. It is not yet clear if we will make use of SimilarityMeasures. 

## Risk analysis

<!-- What could be the biggest challenges/problems you might face? What is your plan B? -->

The research questions are ambitious, as we need to first filter bikers from other means of movement and then find different relevant definitions. As mountainbiking is a relatively "small" movement compared to other movement patterns, it is important to ensure that it doesn't get classified as static and that we don't lose important information. Therefore the first part of this project might be the most crucial, when we define the different parameters. It is for example up do discussion, how we define the relevant turning angles and what sinuosity is relevant.

If we find ourselves overwhelmed with the task, we will shorten our project and try to focus on the detection of bicycle use. 

## Questions?

<!-- Which questions would you like to discuss at the coaching session? -->

Which concept might be more helpful: sinuosity or turning angle?

Will the sample trajectories be comparable? Is there enough data? 

Do we have to many research questions for the scope of this project?
