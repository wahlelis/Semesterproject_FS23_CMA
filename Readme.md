# Proposal for Semester Project

**Patterns & Trends in Environmental Data / Computational Movement Analysis Geo 880**

| Semester:      | FS23                              |
|:---------------|:----------------------------------|
| **Data:**      | Movement data from the class pool |
| **Title:**     | Detecting mountainbikers          |
| **Student 1:** | Aurelia Möri                      |
| **Student 2:** | Lisa Wahlen                       |

## Abstract

<!-- (50-60 words) -->

Mountainbiking is a sport which becomes more and more popular in Switzerland. It is therefore interesting, to assess the behavior and pattern of mountainbikers. This information can not only serve community planning, but also be out of interest for the support of legalization of trails in Switzerland.

Deriving information about where and when people ride mountainbikes can be extracted out of mountainbiking directed apps such as trailforks or strava. But filterin general movement data for mountainbiking patterns could provide more information also about illegal trail uses.

## Research Questions

<!-- (50-60 words) -->

Following this thought, we developped the research questions following below:

-   How can we detect moutainbikers, meaning all bikers riding downhill using gravity offroad?

-   Can we differenciate between different types of mountainbikers? Meaning downhill oriented mountainbiking vs. enduro or even cross-country mountainbiking.

-   How do sinuosity and turning angle influence the speed of bikers?

## Results / products

<!-- What do you expect, anticipate? -->

We expect to...

We expect that the turning angle generally decreases the speed of the bikers.

## Data

<!-- What data will you use? Will you require additional context data? Where do you get this data from? Do you already have all the data? -->

We will use the data from the data - pool of all students of this class. The data has been collected by gps as well as by using the posmo app. For this type of evaluation, the date and time of the collection of the data is irrelevant. The sampling rate on the other hand, is needed to assess the speed.

To detect which are the mountainbike trajectories, we might need a map of some mountainbike trails or a basemap to localize likely mountainbike paths? E.g. movement data within a city might not be part of a mountainbike trail, we assume that mountainbike trails are localised in steep and rural environments.

## Analytical concepts

<!-- Which analytical concepts will you use? What conceptual movement spaces and respective modelling approaches of trajectories will you be using? What additional spatial analysis methods will you be using? -->

## R concepts

<!-- Which R concepts, functions, packages will you mainly use. What additional spatial analysis methods will you be using? -->

We will further use R packages such as dplyr for data wrangling and tidyverse.

We will use R packages from the tidyverse for data wrangling and tidying. Exploratory data analysis and visualisations can be executed with ggplot2. For spatial data we expect to use the packages sf, tmap,

## Risk analysis

<!-- What could be the biggest challenges/problems you might face? What is your plan B? -->

The research questions are ambitious, as we need to first filter bikers from other means of movement and then find different relevant definitions. As mountainbiking is a relatively "small" movement compared to other movement patterns, it is important to ensure that it doesn't get classified as static and that we don't lose important information. Therefore the first part of this project might be the most crucial, when we define the different parameters. It is for example up do discussion, how we define the relevant turning angles and what sinuosity is relevant.

If we find ourselves overwhelmed with the task, we will shorten our project and try to focus on the detection mountainbiking patterns, or even simpler, to differenciate cycling patterns from other kinds of movement patterns.

## Questions?

<!-- Which questions would you like to discuss at the coaching session? -->

Which concept might be more helpful: sinuosity or turning angle?
