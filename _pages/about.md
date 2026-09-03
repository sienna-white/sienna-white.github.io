---
permalink: /
title: "Hello!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi there! 

My name is Sienna White and I am a Ph.D. student at UC Berkeley (2022 - 2027), advised by Professor Mark Stacey. I've written up some of my research experience below. 

I'm grateful to be funded by the Computational Science Graduate Fellowship through the Department of Energy. Please feel free to reach out to me at any time (thoughts on research! potential collaboration! application review for the CSGF! egregious typos on this site!) at _sienna w at berkeley dot edu_ .

Before starting graduate school, I worked at the San Francisco Estuary Institute on the [Clean Water](https://www.sfei.org/programs/projects#) program under Dr. David Senn. Our team used computational models to study nutrient cycling and primary productivity in the Bay Area. We maintained two DFlow-FM hydrodynamic models of San Francisco Bay (one focused on resolving the Sacramento-San Joaquin Delta) coupled to an offline  biogeochemical module (Delft Water Quality, also known as DELWAQ). My work focused mainly on calibrating and validating our model(s) for a range of water years, as well as post-processing model results to communicate with stakeholders.  

Our work is publicly available, but it's ocassinally hard to find, so please reach out if you have any questions or want to learn more -- our work is open source and I'm happy to talk about San Francisco Bay dynamics anytime. 


<!-- **RESEARCH EXPERIENCES:**
----

<span style="color:RebeccaPurple">Predicting harmful algal blooms in the Sacramento-San Joaquin Delta (Dissertation Research)</span>
----

Water quality in the San Francisco Bay Delta affects regional water resources, ecosystem health, and quality of life for any of the two million people who interact with the Delta or call its shores home. However, water management in the Delta has become a heavily politicized issue, as large-scale water withdrawal for agriculture and state water projects often comes at the cost of ecosystem protection measures.

The Delta receives large inputs of anthropogenic nutrients from wastewater treatment plants which result in elevated dissolved inorganic nitrogen levels (Novick et al., 2015). This nutrient-enriched status places the Delta at high risk for algal blooms (Paerl, 2009; Dahm et al., 2016), including risk for bloom events with toxic, or harmful algal species (commonly referred to as harmful algal blooms, or HAB events). These harmful algal blooms threaten public health and endanger the potability of the water supply. Furthermore, climate change, reduced sediment load, and increased nutrient delivery have accelerated algal bloom activity, resulting in increased harmful algal bloom events (Lehman et al., 2017).

My PhD research will focus on using numerical models to investigate the specific mechanisms that precipitate harmful algal blooms, which likely involves a "goldilocks zone" of wind-driven mixing, tidal forcing, river outflow, nutrient supply, and temperature. Better understanding what conditions allow Microcystis (a harmful algal species) to dominate over "beneficial algal species" (diatoms) will then be used to inform a prediction framework, providing water managers with much-needed visibility of where (and when) harmful algal blooms are likely to occur.



---- -->




<!-- 

Sediment transport in San Francisco Bay
----


 * link honors thesis 
 -->

![Fieldwork on San Francisco Bay ](/images/IMG_6533.jpg){width=800px}



 <!-- I'm interested in environmental fluid mechanics, computational fluid modeling, estuarine physics, sediment dynamics ....  benthic grazers ... etc. I finally got around to making a website, so if you found your way here, either on purpose or accident, I'm glad you made it! Feel free to reach out.  -->


<!-- 


Hi there! My name is Sienna White and I am a Ph.D. student at UC Berkeley, working with Professor [Tina Chow](https://chow.ce.berkeley.edu/) on data assimilation for smoke modeling. I'm interested in environmental fluid mechanics, computational fluid modeling, estuarine physics, sediment dynamics ....  benthic grazers ... etc. 

Before I started my PhD at Berkeley, I worked for two years at the San Francisco Estuary Institute on the Clean Water team under Dr. David Senn. At SFEI, I used computational models to study nutrient cycling and primary productivity in the Bay Area. We ran our hydrodynamic model using DFlow-FM and our biogeochemical module was coupled offline using Delft Water Quality (DELWAQ). Our work is publicly available here and here, but it's ocassinally hard to find, so please reach out if you have any questions or want to learn more -- our work is open source and I'm happy to talk about San Francisco Bay dynamics truly anytime !  -->



<!-- 


Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).


<style type="text/css" rel="stylesheet">
.column {
  float: left;
  width: 50%;
  padding: 5px;
}

/* Clear floats after image containers */
.row::after {
  content: "";
  clear: both;
  display: table;
}
</style>

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](../images/editing-talk.png)


For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
