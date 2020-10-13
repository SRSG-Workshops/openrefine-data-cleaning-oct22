---
title: "Introduction"
teaching: 10
exercises: 0
questions:
- "What is OpenRefine useful for?"
objectives:
- "Describe OpenRefine’s uses and applications."
- "Differentiate data cleaning from data organisation."
- "Experiment with OpenRefine’s user interface."
- "Locate helpful resources to learn more about OpenRefine."
keypoints:
- "OpenRefine is a powerful, free and open source tool that can be used for data cleaning."
- "OpenRefine will automatically track any steps you take in working with your data."
---

Why do we need tools like OpenRefine?

- It is important to know what you did to your data as you go on your data journey from data collection to 
data analysis - sometimes you need to modify, reformat or clean your data before you can process it in 
data analysis tools such as R or Python scripts. Additionally, journals,
  granting agencies, and other institutions are requiring documentation of the
  steps you took when working with your data. With OpenRefine, you can capture
  all actions applied to your raw data and share them with your publication as
  supplemental material.
- Any operation that changes the data in OpenRefine can be easily reversed or
  undone.
- Data is often very messy, and OpenRefine saves a lot of time on cleaning
  headaches.
- Data cleaning steps often need repeating with multiple files. OpenRefine is
  perfect for speeding up repetitive tasks by replaying previous actions on
  multiple datasets.
- Some concepts such as clustering algorithms are quite complex (and not available in spreadsheet programmes), 
but OpenRefine
  makes it easy to introduce them, use them, and show their power.
 
## What is OpenRefine and where to find help?
[OpenRefine](http://openrefine.org) is a powerful, free and open source tool with a large growing community of practice. 

  - OpenRefine is a Java program that runs on your machine (not in the cloud): it is a desktop application that uses your web browser as a graphical interface. No internet connection is needed, and none of the data or commands you enter in OpenRefine are sent to a remote server.
  - OpenRefine does not modify your original dataset. All actions are easily reversed in OpenRefine and you can capture all the actions applied to your data and share this documentation with your publication as supplemental material. OpenRefine saves as you go. You can return to the project at any time to pick up where you left off, or export your data to a new file.
 - OpenRefine can be used to standardise and clean data across your files.
    
It can help you:

- Get an overview of a data set
- Resolve inconsistencies in a data set
- Help you split data up into more granular parts
- Match local data up to other data sets
- Enhance a data set with data from other sources
- Save a set of data cleaning steps to replay on multiple files

OpenRefine features:
* Open source ([source on GitHub](https://github.com/OpenRefine/OpenRefine)).
* Has large growing community, from novice to expert, ready to help.
* Works with large-ish datasets (100,000 rows). Does not scale to many millions (yet).

You can read more at <http://openrefine.org> and check out some great [introductory videos](https://www.youtube.com/channel/UCqwSVsJ8CWD9pQUZDbJC1ew). There is a [Google Group](https://groups.google.com/forum/#!forum/openrefine) that can 
answer a lot of beginner questions and problems. 
[OpenRefine recipes, scripts, projects, and extensions](https://github.com/OpenRefine/OpenRefine/wiki/Recipes) are available too, where you can find and copy them into your OpenRefine instance to run on your dataset.

The OpenRefine GitHub wiki page has a [reference](https://github.com/OpenRefine/OpenRefine/wiki/GREL-Functions) of the General Refine Expression Language (GREL) used by OpenRefine (more on GREL in ove of the following episodes).

## Before you get started
 
Make sure you followed the steps in the [Setup section](../setup.html) to install OpenRefine and download data we will 
be using in this lesson.
