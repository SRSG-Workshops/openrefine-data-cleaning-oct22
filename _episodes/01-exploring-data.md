---
title: "Opening and Exploring Data"
teaching: 15
exercises: 10
questions:
- "How can we import our data into OpenRefine?"
- "How can we summarise our data?"
- "How can we find errors in our data?"
objectives:
- "Create a new OpenRefine project from a CSV file."
- "Learn about different types of facets and how they are used to sort and summarise data."
keypoints:
- "Faceting can identify errors or outliers in data."
---

## Creating a project

Start OpenRefine, which will open in your browser (at the address `http://127.0.0.0:3333`). Once OpenRefine is launched in your
browser, the left margin has options to `Create Project`, `Open Project`, or `Import Project`. Here we will create a new
project and import our portal rodents data. 

![OpenRefine Create Project](../fig/openrefine-create-project.png)

1. Click `Create Project` from the left margin and select then `This Computer` (because you're uploading data from your
   computer).  
2. Click `Choose Files` and browse to where you stored the file `Portal_rodents_19772002_scinameUUIDs.csv`. Select the
   file and click `Open`, or just double-click on the filename.
3. Click `Next>>` under the browse button to upload the data into OpenRefine.  
4. On the next screen, OpenRefine will present you with a preview of your data. You can check here for obvious errors,
   if, for example, your file was tab-delimited rather than comma-delimited, the preview would look strange (and you
   could correct it by choosing the correct separator and clicking the `Update Preview` button on the right. If you
   selected the wrong file, click `<<Start Over` at the top left.

    ![OpenRefine Import Data](../fig/openrefine-data-import.png)

4. In the middle of the page, will be a set of options (`Character encoding`, etc.). Make sure the tick box next to
   `Trim leading & trailing whitespace from strings` is not ticked. (We're going to need the leading whitespace in one
   of our examples.) 
5. If all looks well, click `Create Project>>` in the top right. You will be presented with a view onto your data. This
   is OpenRefine!

Let's now start exploring and getting a higher-level overview of our data - summarising and looking for potential 
outliers and errors.

> ## Data file types supported
> OpenRefine can import a variety of different file types, including tab separated (`tsv`), 
> comma separated (`csv`), Excel (`xls`, `xlsx`), JSON, XML, RDF as XML, and Google Spreadsheets. 
> See the [OpenRefine Importers page](https://github.com/OpenRefine/OpenRefine/wiki/Importers) for more information.
{: .callout}

## Data faceting

Facets are one of the most useful features of OpenRefine. Data faceting is a process of exploring data by applying
multiple filters to investigate its composition. It also allows you to identify a subset of data that you wish to change
in bulk.

> ## OpenRefine Wiki: Faceting 
> Full documentation on faceting can be found at [OpenRefine Wiki: Faceting](https://github.com/OpenRefine/OpenRefine/wiki/Faceting)
{: .callout}

### Text facets
A 'text facet' groups all the identical text values in a column and lists each value with the number of records in which
it appears. The facet information always appears in the left hand panel in the OpenRefine interface. We will use text
faceting to look for potential errors in the `scientificName` column.

1. Click the down arrow next to the `scientificName` column.
2. Choose `Facet` > `Text facet`.
3. In the left panel, you'll now see a box containing every unique value in the `scientificName` column 
along with a number representing how many times that value occurs in the column.

    ![OpenRefine Text Facet](../fig/openrefine-text-facet.png)

4. You can click in this panel to sort the facet by `name` and `count`. Do you notice any problems with the data? What
   are they?
5. Hover the mouse over any one of the names in the left panel. You should see that you have an `edit` function
   available. 
6. You could use this to fix an error immediately, and OpenRefine will ask whether you want to make the same correction
   to every value equal to the one you identified. But OpenRefine offers even better ways to find and fix errors across
   the whole dataset, which we will use instead. We will learn about these when we talk about clustering.

There will be several near-identical entries in `scientificName`. For example, there is one entry for `Ammospermophilis harrisi` and
one entry for `Ammospermophilus harrisii`. These are both misspellings of `Ammospermophilus harrisi`. We will see how to correct these 
misspelled and mistyped entries in a later exercise.  

### Other types of facets
As well as 'Text facets' OpenRefine also supports a range of other types of facet. These include:
 
* Numeric facets
* Scatterplot facets
* Timeline facets (for dates)
* Customized facets

**Numeric and scatterplot facets** display graphs instead of lists of values. The numeric facet graph includes 'drag and drop' controls you can use to set a start and end range to filter the data displayed. These facets are explored further in [Examining Numbers in OpenRefine](http://www.datacarpentry.org/OpenRefine-ecology-lesson/03-numbers/).

**Customized facets** are a range of different types of facets, some of which are:

* Word facet - this breaks down text into words and counts the number of records in which each word appears
* Duplicates facet - this results in a binary facet of 'true' or 'false'. Rows appear in the 'true' facet if the value in the selected column is an exact match for a value in the same column in another row
* Text length facet - creates a numeric facet based on the length (number of characters) of the text in each row for the selected column. This can be useful for spotting incorrect or unusual data in a field where specific lengths are expected (e.g. if the values are expected to be years, any row with a text length more than 4 for that column is likely to be incorrect)
* Facet by blank - a binary facet of 'true' or 'false'. Rows appear in the 'true' facet if they have no data present in that column. This is useful when looking for rows missing key data.

Facets are used to group together common values. OpenRefine limits the number of values allowed in a single facet to
ensure the software does not perform slowly or run out of memory. If you create a facet where there are many unique
values (for example, a facet on a 'book title' column in a data set that has one row per book) the facet created will be
very large and may either slow down the application, or OpenRefine will refuse to create the facet.

> ## Exercise
>
> 1. Using faceting, find out how many years are represented in the census (via the `yr` column).  
>
> 2. Is the column formatted as a number, date or text?
>
> 3. Which year has the most and which year has the least observations?
> 
> > ## Solution
> > 
> > 1. For the column `yr` do `Facet` > `Text facet`. A box will appear in the left panel showing that there are 26 unique entries in
> >    this column.  
> > 2. You may have noticed that a numeric facet did not work on the column. By default, the columns in OpenRefine are
> >    formatted as text.
> > 3. You can change the format to numbers by selecting the down arrow next to
> >    the `yr` column name, selecting `Edit cells` > `Common transforms` > `To number`. Notice when this change was
> >    applied that the values in the column changed from black to green, and from left-justified to right-justified. 
> >    If you now select `Facet` > `Numeric facet` on column `yr`, a new box is created that shows a histogram of the number of 
> >    entries per year. Notice that the data is shown as a number, not a date.
> > 4. You can also transform the column to a date by selecting `Edit cells` > `Common transforms` > `To date`. Note the
> >    program will assume all entries take place on 1st January of the year. You can now choose a timeline facet.
> > 5. Click `Sort by count` in the text facet box to order the counts numerically. The year with the most observations
>      is 1997, and the year with the least is 1977. 
> > 
> {: .solution}
{: .challenge}

> ## Default data type 
>
> Be default, all data imported in OpenRefine is treated as text. You have to tell OpenRefine explicitly 
> to treat columns differently via `Edit cells` > `Common transforms`, e.g. as numbers. If you change the 
> data type - it will appear in green. 
>
{: .callout}