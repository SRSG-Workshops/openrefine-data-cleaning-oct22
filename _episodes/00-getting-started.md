---
title: "Introduction"
teaching: 10
exercises: 0
questions:
- "How is OpenRefine useful?"
objectives:
- "Describe OpenRefine’s uses and applications."
- "Differentiate data cleaning from data organisation."
- "Experiment with OpenRefine’s user interface."
- "Locate helpful resources to learn more about OpenRefine."
keypoints:
- "OpenRefine is a powerful and free, open source tool that can be used for data cleaning."
- "OpenRefine will automatically track any steps you take in working with your data."
---

Why do we need a tool like OpenRefine?

- It is important to know what how your data is transformed as you move from data collection to 
data analysis. Sometimes you need to clean your data before you can analyse it. If you don't keep a record of how
you clean the data, you will not be able to reproduce your results - and this is vital if you want to demonstrate how
a result was generated or repeat the analysis later. Reproducibility is becoming increasingly important for journals, funders and other institutions. If you can demonstrate
 every step in your data cleaning and analysis, it is likely to become increasingly difficult to publish results or win
 funding.
  
Manually documenting every data cleaning step is laborious and error prone. With OpenRefine, you can capture
every step automatically, and then easily share the process with collaborators. In addition:
- OpenRefine provides tools that make data cleaning more straightforward, which saves a lot of time.
- It makes powerful but complex processes, such as clustering algorithms, easy to use.
- Any operation in OpenRefine can be easily reversed or undone.
- It is straightforward to repeat a data cleaning process across multiple files - saving even more time.
 
 
## What is OpenRefine and where to find help?
[OpenRefine](http://openrefine.org) is a powerful tool for working with messy data: cleaning it; transforming it from
one format into another.  It provides tools that allow to understand even large data sets, and allows you to get a feel
of the "shape" and content of the data. This helps inform the direction of your later analysis of the data. 
 
It runs in a browser, which might lead you to think that it's a Web or Cloud program. It is not! It is a desktop 
application that uses a browser as convenient interface. No internet connection is needed, and none of your data will be
sent to a remote server.
 
OpenRefine does not modify your original dataset. It stores your raw data set, and presents views on that data set after
applying the data cleaning steps you specify. This means you never lose your original data and you can easily undo
changes. OpenRefine saves as you go, so you can return to the project at any time and pick up where you left off. It
allows you to save the raw data, processed data and all of the data cleaning steps in a file. It also allows you to
export only your processed data to a new file. 
 
OpenRefine is:
* Free.
* Open source ([source on GitHub](https://github.com/OpenRefine/OpenRefine)).
* Has a large growing community, from novice to expert, ready to help.
* Works with large-ish datasets (100,000 rows), but does not yet scale to many millions of rows.

Click the arrow in the bottom right of the page to proceed to the next lesson.

## Further reading

You can find out more on the [OpenRefine website](http://openrefine.org) and check out some great [introductory videos](https://www.youtube.com/channel/UCqwSVsJ8CWD9pQUZDbJC1ew). There is a [Google Group](https://groups.google.com/forum/#!forum/openrefine) that can 
answer a lot of beginner questions and problems. 
[OpenRefine recipes, scripts, projects, and extensions](https://github.com/OpenRefine/OpenRefine/wiki/Recipes) are available too, where you can find useful transformations to run on your own data.

The OpenRefine GitHub wiki page has a [reference](https://github.com/OpenRefine/OpenRefine/wiki/GREL-Functions) of the General Refine Expression Language (GREL) used by OpenRefine (more on GREL in ove of the following episodes).