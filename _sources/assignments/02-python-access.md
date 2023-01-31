---
substitutions:
  accept_assignment: |
    [accept the assignment]()
  date : 20yy-mm-dd
---
# Assignment 2: Practicing Python and Accessing Data


due : {{ date }}

## Objective & Evaluation
Eligible skills: (links to checklists)
- **first chance** prepare [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#prepare-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#prepare-level2)
- access [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#access-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#access-level2)
- python [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#python-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#python-level2)
- summarize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level1) 
This assignment is an opportunity to earn level 1 and 2 achievements in `python` and `access` and begin working toward level 1 for `summarize`. You can also earn level 1 for `process`.

In this assignment, you'll practice/ review python skills by manipulating datasets
and extracting basic information about them.

## Related notes

- [](../notes/2023-01-31)
- [](../notes/2023-02-02)




## Setting

Next week, we are going to learn about summarizing data. In this assignment, you are going to build a small dataset about datasets. In class next week, we will combine all of your datasets about datasets together in order to be able to answer questions like:

- how much total data did you all load
- how many students picked the same dataset?
- how many total rows of data did each student load?




First, {{ accept_assignment }}. It contains a notebook with some template structure (and will set you up for grading).


## Find Datasets

Find 3 datasets of interest to you that are provided in at least two different file formats. Choose datasets that are not too big, so that they do not take more than a few second to load. At least one dataset, must have non numerical (eg string or boolean) data in at least 1 column.

In your notebook, create a markdown cell for each dataset that includes:
- heading of the dataset's name
- a 1-2 sentence summary of what the dataset contains and why it was collected
- a "more info" link to where someone can learn about the dataset
- 1-2 questions you would like to answer with that dataset.

## Store them for loading

Create a list of dictionaries in `datasets.py`, so that there is one dictionary for each dataset. Each dictionary should have the following keys:

```{list-table} Meta Data Description of the dictionary to create
:header-rows:0

*- `url`
  - with the url
* - `short_name`
  - a short name
* - `load_function`
  - (the actual function handle) what function should be used to load the data into a `pandas.DataFrame`.

```

## Make a dataset about your datasets

````{margin}
```{hint}
See they [python module docs for examples](https://docs.python.org/3/tutorial/modules.html#modules)
```
````
In a notebook called `dataset_of_datasets.ipynb`, import the list of dictionaries from the `datasets` module you created in the step above. 
Then {term}`iterate` over the list of dictionaries, and:  

1. save it to a local csv using the short name you provided for the dataset as the file name, without writing the index column to the file.
1. record attributes about the dataset as in the table below in a list of lists or dictionary
1. Use that to create a DataFrame with columns that match the rows of the following table.

```{list-table} Meta Data Description of the DataFrame to build
:header-rows:0

* - name
  - a short name for the dataset
* - source
  - a url to where you found the data
* - num_rows
  - number of rows in the dataset
* - num_columns
  - number of columns in the dataset
* - num_numerical
  - number of numerical variables in the dataset
```

## Explore Your Datasets

In a second notebook file called `exploration.ipynb`: 

For one dataset that includes nonnumerical data:
- read it in from your local csv using a relative path
- display the heading and the last 4 rows
- make a numpy array of only the numerical data and save it to a new variable (select these programmatically)
- was the format that the data was provided in a good format? why or why not?


For any other dataset:
- read it in from your local csv using a relative path
- display the heading with the first three rows
- display the datatype for each column
- Are there any variables where pandas may have read in the data as a datatype that's not what you expect (eg a numerical column mistaken for strings)? If so, investigate and try to figure out why.

For the third dataset:
- read it in from your local csv using a relative path
- display the first 3 multiples of 3 rows (eg 3,6,9) of the data for two columns of your choice

## Exploring data files

There are two files in the data folder, both can be read in with `read_csv` but need some options or fixing.

- try to read in the `german.data` file, what happens with the default settings? What option do you need to use to make it look right?
- try to read in the `.csv` file that's included in the template repository (), use the error messages you get to try to fix the file manually (any text editor, including jupyter can edit a `.csv`), making notes about what changes you made in a markdown cell.



## Submission

```{important}
This is TBA instructins will be here on Thursday
```

## Thinking ahead

```{important}
This section is not required, but is intended to help you get started thinking
about ideas for your portfolio.  If you complete it, we'll give your feedback to
help shape your ideas to get to level 3 achievements.  If you want to focus only
on level 2 at this moment in time, feel free to skip this part. You could also think about this after submitting the assignment, since you do not have to get a grade for it. If you want, you could discuss these ideas in office hours.
```


1. When might you prefer one datatype over another?
1. How does PEP 8 standard code help you be collaborative?
1. Learn about [Datasheets for Datasets](https://arxiv.org/pdf/1803.09010.pdf) and find some examples, (eg this [google scholar result](https://scholar.google.com/scholar?q=datasheets+for+datasets&hl=en&as_sdt=0&as_vis=1&oi=scholart) ) How could something like this impact your work as a data scientist?
