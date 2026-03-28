---
title: "Research"
layout: single
classes: wide academic-page research-page
excerpt: "Research themes and current projects in mountain snow hydrology, SWE modeling, and remote sensing."
permalink: /research/
author_profile: false
header:
  overlay_filter: 0.48
  overlay_image: /assets/images/yosemite_winter_nps.png
  overlay_excerpt: >
    Current projects and research highlights in mountain snow hydrology, SWE modeling,
    and applied remote sensing.





---

<section class="research-sticky-layout">
  <div class="research-sticky-layout__intro">
    <section class="academic-intro">
      <div class="section-heading">
        <p class="section-heading__eyebrow">Research Direction</p>
        <h2>Improving our understanding of mountain snowpack dynamics across scale.</h2>
      </div>
      <p class="academic-intro__lead">
        My research aims to improve our understanding of mountain snowpack dynamics and develop
        better model representations of snow water resources in complex terrain. Currently, I am most
        interested in developing downscaling techniques for global SWE products.
      </p>
      <div class="chip-row">
        <span class="chip">Improving SWE model estimates in mountainous basins</span>
        <span class="chip">Remote sensing for SWE estimation</span>
        <span class="chip">Downscaling SWE and snowfall from global reanalysis</span>
        <span class="chip">Snow processes in glacier mass-balance modeling</span>
      </div>
    </section>
  </div>

  <div class="research-sticky-layout__cards">
    <section class="project-feature">
      <div class="section-heading">
        <p class="section-heading__eyebrow">Current Project</p>
        <h2>Modeling SWE at continental scales</h2>
      </div>
      <p class="project-meta">2022-2026 | NASA Grant #80NSSC22K0585</p>
      <p>
        The <strong>Co</strong>ld <strong>Re</strong>gions <strong>S</strong>nowfall and
        <strong>S</strong>nowpack <strong>D</strong>ataset (CoReSSD) is a 1 km snowfall and snow
        water equivalent dataset spanning North America above 30°N for water years 2001-2021.
        This dataset was produced with funding from NASA Grant #80NSSC22K0585. CoReSSD relies on the
        Blender algorithm (Dechow et al., 2026, <em>Water Resources Research</em>), a non-linear
        optimization technique that recomputes the modeled mass and energy balance of the snowpack
        while being constrained by remotely sensed snow cover fraction.
      </p>
      <p>
        I was involved in the development and testing of the Blender algorithm during my PhD at Ohio State
        University and continued that work during my postdoc at UNC. At UNC, I helped update the algorithm
        to run more efficiently over large domains, developed the precipitation scaling technique used to
        improve spatial variability in the prior dataset, and oversaw production of the full dataset.
      </p>
    </section>

    <section class="feature-figure">
      <figure>
        <img src="/assets/images/CSD_AGU_WY16_final.jpg" alt="CoReSSD SWE across the western United States, March 15 2016" />
        <figcaption>
          CoReSSD snow water equivalent across the western United States on March 15, 2016.
          The Sierra Nevada, Cascades, and Rockies remain visually distinct even in a broad-domain product.
        </figcaption>
      </figure>
      <div class="feature-figure__content">
        <p class="section-heading__eyebrow">Research Highlight</p>
        <h2>CoReSSD: a 1 km North American SWE dataset</h2>
        <p>
          Initial validation against the Western U.S. Snow Reanalysis (WUS; Fang et al., 2022)
          shows CoReSSD substantially outperforms both the NoahMP prior (R = 0.71, RMSE = 83.1 mm)
          and ERA5-Land (R = 0.63, RMSE = 90.9 mm), achieving R = 0.89 and RMSE = 56.2 mm in the
          test basin.
        </p>
        <p>
          Full validation across the 20-year record is ongoing and is being prepared for submission
          to <em>Earth System Science Data</em>.
        </p>
      </div>
    </section>

    <section class="feature-figure feature-figure--reverse">
      <figure>
        <img src="/assets/images/denali_wolf.png" alt="Wolf movement rates before, during, and after the storm." />
        <figcaption>
          Example of how snow and ice conditions can be linked to ecological response during extreme winter events.
        </figcaption>
      </figure>
      <div class="feature-figure__content">
        <p class="section-heading__eyebrow">Interdisciplinary Application</p>
        <h2>Snow modeling beyond hydrology</h2>
        <p>
          In December 2021, an atmospheric river dropped a 300-year precipitation event on interior Alaska,
          more than 7 SD above the 99-year mean at Denali National Park. Using snow pit surveys across forest,
          shrub, and tundra sites, we found that ice thickness within the snowpack varied dramatically by
          vegetation type, and caribou shifted to higher elevations to find accessible forage.
        </p>
        <p>
          These results suggest that topographic and habitat diversity in mountainous ecosystems may buffer
          wildlife populations against even extreme winter weather events. I contributed the land surface and
          passive microwave snow modeling used to characterize the spatial extent and intensity of the
          rain-on-snow event across the park.
        </p>
      </div>
    </section>
  </div>
</section>
