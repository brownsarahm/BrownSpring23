# Assignment 9: Linear Regression

## Quick Facts
- [accept the assignment](https://classroom.github.com/a/kUmNgzdA)
- __Due: 2023-04-04__


## Assessment

Eligible skills: (links to checklists)


- **first chance** regression [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#regression-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#regression-level2)
- process [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#process-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#process-level2)
- evaluate [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level2)
- summarize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level2)
- visualize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level2)



## Related notes

- [](../notes/2023-03-28)
- [](../notes/2023-03-30)


## Instructions

Find a dataset suitable for regression. We recommend a dataset from the UCI repository.

### Linear Regression Basics

TLDR: Fit a linear regression model, measure the fit with two metrics, and make a plot that helps visualize the result.

1. Include a basic description of the data(what the features are)
1. Write  your own description of what the prediction task it, why regression is appropriate.
1. Fit a linear model on all relevant features with 75% training data.
1. Test it on 25% held out test data and measure the fit with two metrics and one plot
1. Inspect the model to answer:

    - Does this model make sense?
    - What to the coefficients tell you?
    - What to the residuals tell you?
1. Repeat the split, train, and test steps 5 times.

    - Is the performance consistent enough you trust it?
1. Interpret the model and its performance in terms of the application. Some questions you might want to answer in order to do this include:

  - do you think this model is good enough to use for real?
  - is this a model you would trust?
  - do you think that a more complex model should be used?
  - do you think that maybe this task cannot be done with machine learning?
1. Try fitting the model only on one feature. Justify your choice of feature based on the results above.  Plot this result.



### Part 2: Exploring Evaluation

````{margin}
```{tip}
The summary statistics and visualization we used before are useful for helping to
investigate the performance of our model.  We can try fitting a model  with different settings
to create a new "dataset" for our experiments.
The same skills apply.
```
````


Do an experiment to compare test set size vs performance:
1. Train a regression model on 10%, 30%, ... , 90% of the data. Save the results of both test and train performance for each size training data in a DataFrame with columns ['train_pct','n_train_samples','n_test_samples','train_r2','test_r2']
1. Plot the performance vs training percentage in a line graph.  
1. Interpret these results.  How does training vs test size impact the model?



```{admonition} Thinking Ahead

Try these experiments with a different type of regression.

```
