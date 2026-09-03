---
title: "Project Two: A Short, Descriptive Title"
collection: research
permalink: /research/smoke/
slug: smoke
excerpt: "Data assimilation for a high-resolution PM2.5 analysis dataset"
order: 2
accent: "pink"
figure: "/images/500x300.png"
figure_caption: "Figure 1: Replace this placeholder with a key figure, schematic, or result from this project."
github: "https://github.com/siennarwhite/your-repo-name"
paperurl: ""
---

**Overview.** During my first year at UC Berkeley (2021-2022), I worked with Prof. Tina Chow and Dr. Rebecca Sugrue. I worked on “Partnering for Resilient Opportunities To Eliminate Cumulative Toxic (PROTECT) Health Effects from Wildfire PM2.5 in Environmental Justice Communities,” an EPA Region 9 grant involving a consortium of scientists from Berkeley, LBNL, and UCSF. The overreaching goal of this grant was to explore how long-term exposure to wildfire smoke has impacted public health in environmental justice communitiies. In order to do so, our team focused on assimilating observational data into modeled wildfire smoke fields to generate an hourly “best guess” of smoke concentrations across California from 2016-2020. These results were then passed off to public health researchers for exposure analysis. You can learn more about the overall grant here. For me, it was a great opportunity work directly with researchers in the public health/medical space and gain a broader persepctive on the utility (and lack thereof) of numerical modeling for providing input data to other disciplines.


![PM_{2.5} concentrations vary significantly over a 24-hour period, especially during wildfire smoke episodes.](/images/smoke/cover_est.jpeg)


**Methods / Approach.** Describe your methods, models, or data sources here.

**A sample equation.**

$$
\hat{y} = \beta_0 + \sum_{i=1}^{n} \beta_i x_i + \varepsilon
$$

Replace with the relevant formulation for this project.

**Status & next steps.** Note what's done, what's in progress, and what's next.

Tip: leave `paperurl` blank (as above) if there's no publication yet — the "Read the paper" button will simply not appear until you add a link.


PM$_{2.5}$ concentrations can vary dramatically over the course of a day, especially during wildfire smoke events. This image depicts the 100 μg/m3 PM2.5 contour throughout September 7, 2020 in Southern California, in the midst of the historic 2020 wildfire season. These estimates of PM2.5 were developed using data assimilation, a data fusion process that combines observational and numerical model data. The rapidly changing air quality concentrations demonstrate that high frequency PM2.5 estimates may be a critical tool to better understand how sub-daily PM2.5 exposure affects public health.



<span style="color:DarkSeaGreen">Data assimilation for wildfire smoke models</span>
----

During my first year at UC Berkeley (2021-2022), I decided to try my hand at atmospheric modeling and was lucky enough to do so under the mentorship of [Prof. Tina Chow](https://chow.ce.berkeley.edu) and Dr. Rebecca Segrue. I worked on _"Partnering for Resilient Opportunities To Eliminate Cumulative Toxic (PROTECT) Health Effects from Wildfire PM2.5 in Environmental Justice Communities,"_ an EPA Region 9 grant involving a consortium of scientists from Berkeley, LBNL, and UCSF. The overreaching goal of this grant was to explore how long-term exposure to wildfire smoke has impacted public health in environmental justice communitiies. In order to do so, our team focused on assimilating observational data into modeled wildfire smoke fields to generate an hourly "best guess" of smoke concentrations across California from 2016-2020. These results were then passed off to public health researchers for exposure analysis. You can [learn more about the overall grant here](https://cfpub.epa.gov/ncer_abstracts/index.cfm/fuseaction/display.abstractDetail/abstract_id/11358/report/0). For me, it was a great opportunity work directly with researchers in the public health/medical space and gain a broader persepctive on the utility (and lack thereof) of numerical modeling for providing input data to other disciplines. 

### Background on data assimilation

Data assimilation is a statistical exercise that attempts to address the very useful question of "how can we combine observational data with model results when we know there are errors in both methods?" (If it's useful to anyone, I might come back later and add a better explanation here -- please reach out!). It's commonly employed in weather forecasting, as weather forecasts have extraordinary sensitivity to their initial condition -- so everytime you restart a weather model, it makes sense to check what your model is saying and what measurements-on-the-ground report. I found this [paper by Ahmed et al. (2020)](https://www.osti.gov/pages/servlets/purl/1737509) to be a very accessible, well-explained walkthrough on what this looks like mathematically.  

As it turns out, unbeknownest to me, meteorologists have mastered data assimilation for both static fields (e.g., generating intial conditions) with all sorts of data, including satellite irradiance and weather balloon data with a host of methodologies (3-D Var, Ensemble Kalman Filter, etc) Beyond looking at a snapshot in time, there's also a data assimilation practice known as "4D-Var" which incorporates observational data into a model as it's running. For this exercise, I stuck to the simplest possible implementation of data assimilation, and with the very patient guidance of our collaborators at NOAA was able to deploy the Gridpoint Statistical Interpolation tool (GSI) for 3D-Var assimilation.


![HRRR-Smoke model field plotted alongside EPA AirNow sensor data.](/images/HRRR-Smoke concentration plotted with AQS obs data at November 09, 2018 at 09_00 (before DA).png)


![Comparing pre v post assimilation PM25 at September 06, 2020 at 00_00.](images/smoke/Comparing pre v post assimilation PM25 at September 06, 2020 at 00_00.png)

### Our methodology

For our "background field" (e.g, initial model result) we used simulations from HRRR-Smoke, an implementation of the high-resolution rapid refresh model that includes smoke as a tracer. We started with raw GRIB2 model output and used WPS/WRF utilites to prepare an input file for GSI. Most of this work involved developing efficient pipelines for processing enormous quantities of data. We then assimilated observational data from EPA AirNow sensors as well as Purple Air. (One ongoing question of this research involves how best to quantify the observational error in Purple Air sensors when assimilation these data into the modeled smoke field.) You can see an example of this assimilated smoke field here. 



![Results of data assimilation on the wildfire smoke / PM2.5 field](/images/Comparing pre v post assimilation PM25 at November 09, 2018 at 09_00.png)


If this dataset is interesting to you, or if you'd like me to share the python repositories I developed to perform and automate this process, please reach out. 


