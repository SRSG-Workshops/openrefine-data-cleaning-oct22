---
layout: page
title: Setup
---

## Data  
The data used in this lesson comes from a project observing a small mammal community in southern 
Arizona, US. This is part of a project studying the effects of rodents and ants on the plant 
community that has been running for almost 40 years. The rodents are sampled on a series of 24 plots, 
with different experimental manipulations controlling which rodents are allowed to access which plots.
 
This is a real dataset that has been used in over 100 publications. We have simplified it just a 
little bit for the purposes of this lesson, but you can download the full dataset and work with it using exactly the same tools we will learn here. This simplified version of data is available to download 
from the [Portal Project Teaching Dataset available on Figshare](http://figshare.com/articles/Portal_Project_Teaching_Database/1314459).
The original database is published at [Ecological Archives](http://esapubs.org/archive/ecol/E090/118/) and this version of the database should be used for research purposes. 
 
> ## Portal Project Teaching Dataset
> [The Portal Project Teaching Database](http://figshare.com/articles/Portal_Project_Teaching_Database/1314459) is a simplified version of the 
> [Portal Project Database](https://github.com/weecology/PortalData) designed for teaching. It provides a real world example of life-history, population, and ecological data, with sufficient complexity to teach many aspects of data analysis and management, but with many complexities removed to allow students to focus on the core ideas and skills being taught. The database is currently available in csv, json, and sqlite formats.
> 
> The Portal Project Teaching Database's GitHub repository can be found at: [https://github.com/weecology/portal-teachingdb](https://github.com/weecology/portal-teachingdb), 
> where suggested changes or additions to this dataset can be requested or contributed. 
> This database is not designed for research as it intentionally removes some of the real-world complexities. The Python code used for converting the original database to this teaching version can be found in [create_portal_teach_dataset.py](https://github.com/weecology/portal-teachingdb/blob/master/create_portal_teaching_dataset.py). 
>
> **CITATION:** Ernest, Morgan; Brown, James; Valone, Thomas; White, Ethan P. (2017): Portal Project Teaching Database. Figshare. [https://doi.org/10.6084/m9.figshare.1314459.v6](https://doi.org/10.6084/m9.figshare.1314459.v6)
{: .testimonial}

In this lesson, we will use the following file from the [Portal Project Teaching Dataset](http://figshare.com/articles/Portal_Project_Teaching_Database/1314459). You should download it as a preparation for the workshop.
-  [Portal_rodents_19772002_scinameUUIDs.csv](https://ndownloader.figshare.com/files/7823341) 

## Software

For this lesson you will need [OpenRefine](http://openrefine.org/) (formerly GoogleRefine) and a web browser.

[OpenRefine](http://openrefine.org/) is a Java program that runs locally on your machine (i.e. you are not accessing a remote service on the 
Internet). You access it via your browser, but no Internet connection is needed.


### Windows

- If you have Internet Explorer (or Edge) set as your default web browser, check that you have Firefox or Chrome installed and set either of them as your 
default browser. OpenRefine runs in your default browser, but may not run correctly in Internet Explorer.
 - Learn how to set your browser as default by clicking on this link for [Google Chrome](https://support.google.com/chrome/answer/95417?co=GENIE.Platform%3DDesktop&hl=en-GB) and this link for [Firefox](https://support.mozilla.org/en-US/kb/make-firefox-your-default-browser).
- Download software from [OpenRefine](http://openrefine.org/download.html)
 - Select the most recent version of OpenRefine (do not select beta versions or the release candidates). The version that you should download will be at the top of the page and named OpenRefine 3.1 for example.
- Unzip the downloaded file into a directory by right-clicking and selecting “Extract…”. Name that directory something like OpenRefine.
- Go to your newly created OpenRefine directory.
- Launch OpenRefine by clicking on openrefine.exe (this will launch a command prompt window first; ignore that, and wait for OpenRefine to launch in the web browser, which is where you will interact with the program).
- If you are using a different browser, or OpenRefine does not automatically open for you, point your browser at http://127.0.0.1:3333/ or http://localhost:3333 to launch the program.

### Mac

- Check that you have Firefox or Chrome browsers installed and set as your 
default browser. OpenRefine runs in your default browser. It will not run correctly in Internet Explorer.
- Download software from [OpenRefine](http://openrefine.org/download.html)
- Select the most recent version of OpenRefine (do not select beta versions or the release candidates). The version that you should download will be at the top of the page and named OpenRefine 3.1 for example.
- Unzip the downloaded file into a directory by double-clicking it. Name 
that directory something like OpenRefine.
- Go to your newly created OpenRefine directory.
- Launch OpenRefine
- Drag icon into Applications folder, and Ctrl-click/Open… it. 
- If you are using a different browser, or OpenRefine does not automatically open for you, point your browser at http://127.0.0.1:3333/ or http://localhost:3333 to launch the program.

### Linux

- Check that you have Firefox or Chrome browsers installed and set as your 
default browser. OpenRefine runs in your default browser. It will not run correctly in Internet Explorer.
- Download software from [OpenRefine](http://openrefine.org/download.html)
- Select the most recent version of OpenRefine (do not select beta versions or the release candidates). The version that you should download will be at the top of the page and named OpenRefine 3.1 for example.
- Unzip the downloaded file into a directory. Name that directory something like OpenRefine.
- Go to your newly created OpenRefine directory.
- Launch OpenRefine
- Type ./refine into the terminal within the OpenRefine directory
- If you are using a different browser, or OpenRefine does not automatically open for you, point your browser at http://127.0.0.1:3333/ or http://localhost:3333 to launch the program.

