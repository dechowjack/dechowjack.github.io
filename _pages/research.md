---
title: "Research"
layout: single
excerpt: ""
permalink: /research/
author_profile: true
header:
  overlay_filter: 0.3
  overlay_image: /assets/images/yosemite_winter_nps.png





---

<!-- TODO: Write a 2-3 sentence overview of your research program here -->

My research aims to improve our understanding of mountain snowpack dynamics and develop
better model representations of snow water resources in complex terrain. Currently, I am most interested in developing downscaling techniques for global SWE products.

Some of my specific research interests include:

- Improving SWE model estimates in complex, mountainous basins
- Developing scalable methods for snow water equivalent estimation from remote sensing
- Development of downscaling methods for SWE and snowfall estimates from global reanalyis datasets
- Improving snow process representation in glacier mass-balance modeling

# Research Projects

## The *Co*ld *Re*gions *S*nowfall and *S*nowpack *D*ataset (CoReSSD)

**[2022-2026] | NASA Grant #80NSSC22K0585**
The Cold Regions Snowfall and Snowpack Dataset (CoReSSD) is a 1 km snowfall and snow water equivalent dataset. CoReSSD covers the entirety of North American above 30°N for water years 2001-2021. This dataset was produced with funding from NASA Grant #80NSSC22K0585. CoReSSD relies on the Blender algorithm (Dechow et al., 2026, Water Resources Research). Blender is a non-linear optimization technique to recompute the modeled mass and energy balance of the snowpack, constrained by remotely sensed snow cover fraction. Blender requires a prior estimate, i.e. initial conditions, of the snowpack mass and energy balance. The original Blender algorithm paper can be found below.

I was involved in the development and testing of the Blender algorithm during my PhD at Ohio State University. Following my PhD, I continued work on the project during my postdoc at UNC. At UNC, I helped with development of the updated Blender algorithm to be more efficient running over large domains. I also developed the precipitation scaling technique used to improve spatial variability in the prior dataset. Finally, I oversaw the production of the entirety of the dataset, and am currently working through the initial validation of results.

---

# Research Highlights

## CoReSSD: A 1 km North American SWE Dataset

![CoReSSD SWE across the western United States, March 15 2016](/assets/images/CSD_AGU_WY16_final.png)
The map above shows CoReSSD SWE on March 15, 2016 across the western United States. The Sierra Nevada and Cascades are clearly visible along the left; the Rockies appear on the right. SWE values exceeding 1 m (green to yellow) are concentrated along high-elevation ridgelines, while lower-elevation areas show the thin snowpack typical of that water year. The magenta outline marks the Rio Grande National Forest, the primary validation basin for this work.

Initial validation against the Western U.S. Snow Reanalysis (WUS; Fang et al., 2022) shows CoReSSD substantially outperforms both the NoahMP prior (R = 0.71, RMSE = 83.1 mm) and ERA5-Land (R = 0.63, RMSE = 90.9 mm), achieving R = 0.89 and RMSE = 56.2 mm in the test basin. Full validation across the 20-year record is ongoing and will be submitted to *Earth System Science Data*.

## Interdisciplinary applications of snow modeling

Image example:
![Wolf movement rates before, during, and after the storm.](/assets/images/denali_wolf.png)
In December 2021, an atmospheric river dropped a 300-year precipitation event on interior Alaska, more than 7 SD above the 99-year mean at Denali National Park. Despite conditions that might be expected to cause mass wildlife die-offs, caribou and wolf populations showed a surprisingly muted demographic response. Using snow pit surveys across forest, shrub, and tundra sites, we found that ice thickness within the snowpack varied dramatically by vegetation type, and caribou shifted to higher elevations to find accessible forage. These results suggest that topographic and habitat diversity in mountainous ecosystems may buffer wildlife populations against even extreme weather events. I contributed the land surface and passive microwave snow modeling used to characterize the spatial extent and intensity of the rain-on-snow event across the park.
1
