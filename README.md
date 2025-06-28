# syria_pop
# Reasoning

In some of the work I do, I look at geographic boundaries and population estimates for Syria. Compared to ten years ago, there are several sources of open-source data thanks to communities like Open Street Map's Humanitarian OSM Team (HOT) and the UN OCHA's [Humanitarian Data Exchange](https://data.humdata.org/). But, how do these population estimates compare? What affects their accuracy? Are there scenarios where one estimate source is better to use than another?

Since I've spent time doing this work already *and* I always love an excuse to play with geopandas and other map-based visuals, I created this repo to share the code and results of this research.

## OSM Data
source: [HDX HOTOSM Syria](https://data.humdata.org/dataset/hotosm_syr_populated_places)

Missing administrative boundaries data so I added them by joining to UN's administrative boundaries data.

Data is crowdsourced via volunteers contributing to the HOT's mapping.

## Assistance Coordination Unit (ACU) Data
source: [HDX ACY Syria](https://data.humdata.org/dataset/hotosm_syr_populated_places)

Just for northeast Syria from October 2024 which is limited but also shows a trend reflected in other aid agencies' work. Namely, that they did not cover areas in northeast Syria that were controlled by the Assad-led Syrian government at the time, contributing to a substantial gap in information for 8 subdistricts in northeast Syria.  

Data is collected by field team observing IDP movements and population. (this needs more info... are they using pre-existing census data from an earlier time?)

## World Pop data
source: [HDX World Population Syria](https://data.humdata.org/dataset/worldpop-population-counts-2015-2030-syr)
Spatially distributed via random forest so it's great for high level over view such as per governorate. Not as useful for town-level population estimates.

I used the 2025 estimates. 

Its estimates were on average X% higher then OSM or ACU.

# Visuals

# When to use what

