---
layout: page
title: Setup
---

## Data  
The data used in this lesson comes from a project observing a small mammal community in southern
Arizona, US. This is part of a project studying the effects of rodents and ants on the plant
community that has been running for almost 40 years. The rodents are sampled on a series of 24 plots,
with different experimental manipulations controlling which rodents are allowed to access which plots.

The Portal Project Teaching Dataset is a real dataset that has been used in over 100 publications. We have simplified it
for the purposes of this lesson, but you can download the full dataset (see below for details) and work with it
using exactly the same tools we will learn here.
 
For this lesson, you will need to download the following file (remember where you downloaded the file!):
*  [Portal_rodents_19772002_scinameUUIDs.csv](https://ndownloader.figshare.com/files/7823341)

Data in some of the columns of the above file (namely `locality`, `county`, `country`, `JSON`, `decimalLatitude` and `decimalLongitude`) are contrived for the purpose of the lessons and are in no way related to the original dataset. 

> ## For Interest Only: Portal Project Teaching Dataset
> [The Portal Project Teaching Database](http://figshare.com/articles/Portal_Project_Teaching_Database/1314459) is a simplified version of the 
> [Portal Project Database](https://github.com/weecology/PortalData) designed for teaching. It provides a real world example of life-history, population, and ecological data, with sufficient complexity to teach many aspects of data analysis and management, but with many complexities removed to allow students to focus on the core ideas and skills being taught. The database is currently available in csv, json, and sqlite formats.
> 
> The Portal Project Teaching Database's GitHub repository can be found at: [https://github.com/weecology/portal-teachingdb](https://github.com/weecology/portal-teachingdb), 
> where suggested changes or additions to this dataset can be requested or contributed. 
> This database is not designed for research as it intentionally removes some of the real-world complexities. The Python code used for converting the original database to this teaching version can be found in [create_portal_teach_dataset.py](https://github.com/weecology/portal-teachingdb/blob/master/create_portal_teaching_dataset.py). 
>
> **CITATION:** Ernest, Morgan; Brown, James; Valone, Thomas; White, Ethan P. (2017): Portal Project Teaching Database. Figshare. [https://doi.org/10.6084/m9.figshare.1314459.v6](https://doi.org/10.6084/m9.figshare.1314459.v6)
{: .testimonial}

## Now what?

Once you've downloaded the file above, you can [start the lesson](https://southampton-rsg.github.io/openrefine-data-cleaning/00-getting-started/index.html).

<!--
## Software

For this lesson you will need [OpenRefine](http://openrefine.org/) (formerly GoogleRefine) and a web browser.

Download the most recent version of [OpenRefine](http://openrefine.org/download.html) for your operating system, 
then follow instructions below.

[OpenRefine](http://openrefine.org/) is a Java program that runs locally on your machine (i.e. you are not accessing a remote service on the Internet). You access it via your browser, but no Internet connection is needed. Most recent versions of 
OpenRefine come with embedded Java so you do not even have to worry whether you have Java on your system or not.


### Windows
- If you have Internet Explorer (or Edge) set as your default web browser, check that you have Firefox or Chrome installed and set either of them as your default browser. OpenRefine runs in your default browser, but may not run correctly in Internet Explorer. You can check how to set your browser as default for [Google Chrome](https://support.google.com/chrome/answer/95417?co=GENIE.Platform%3DDesktop&hl=en-GB) or [Firefox](https://support.mozilla.org/en-US/kb/make-firefox-your-default-browser).
- Unzip the downloaded file into a directory by right-clicking and selecting `Extract...`. Name that directory something like OpenRefine.
- Locate `openrefine.exe` in the extracted folder and launch OpenRefine by double-clicking on it. This will launch a command prompt window first; ignore that, and wait for OpenRefine to launch in your default Web browser, which is where you will interact with the program.
- If a Web browser does not automatically open for you upon launch, type the following URL in your browser: 
[http://127.0.0.1:3333/](http://127.0.0.1:3333/) or [http://localhost:3333](http://localhost:3333) to launch the program.

### Mac

- Check that you have Firefox or Chrome browser installed and set as your default browser. 
- Locate the downloaded `.dmg` file and Ctrl-click it. You may get the warning "macOS cannot verify the developer of “OpenRefine.app”. Are you sure you want to open it?" Click 'Yes'/'Open' to this. 
- Drag `OpenRefine.app` into your Applications folder, and Ctrl-click to open it. You may get the warning "macOS cannot verify the developer of “OpenRefine.app”. Are you sure you want to open it?" Click 'Yes'/'Open' to this. 
- If a Web browser does not automatically open for you upon launch, type the following URL in your browser: 
[http://127.0.0.1:3333/](http://127.0.0.1:3333/) or [http://localhost:3333](http://localhost:3333) to launch the program.


### Linux

- Check that you have Firefox or Chrome browser installed and set as your default browser. 
- Unzip the downloaded file into a directory. Name that directory something like OpenRefine.
- Go to your newly created OpenRefine directory.
- Type ./refine into the terminal within the OpenRefine directory
- If a Web browser does not automatically open for you upon launch, type the following URL in your browser: 
[http://127.0.0.1:3333/](http://127.0.0.1:3333/) or [http://localhost:3333](http://localhost:3333) to launch the program.

-->
