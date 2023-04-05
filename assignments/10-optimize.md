
# Assignment 10: Tuning Model Parameters

## Quick Facts
- [accept the assignment](https://classroom.github.com/a/5YuJzvVi)
- __Due: 2023-04-11__

## Related notes

- [](../notes/2023-04-04)
- [](../notes/2023-04-06)

## Assessment

Eligible skills: (links to checklists)
- **first chance** optimization [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#optimization-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#optimization-level2)
- clustering [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#clustering-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#clustering-level2)
- regression [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#regression-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#regression-level2)
- classification [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#classification-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#classification-level2)
- evaluate (must use extra metrics to earn this here) [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level2)
- summarize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level2)
- visualize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level2)


## Instructions

**summary** Extend the work you did in assignment 7,8, or 9, by optimizing the model parameters.

1. Choose your dataset, task, and a model. It can be any model we have used in class so far. Include a breif description of the task(this can be copied from 7,8, or 9 if applicable but please include it for completeness).
1. Fit the model with default parameters and check the score. Interpret the score in context. (again can be reused)
2. Choose reasonable model parameter values for your parameter grid by assessing how well the model fit with the default values.
3. Use grid search to find the best performing model parameters.
4. Examine the best fit model, how different is it from the default?  Score the best fit model on a held out test set.
5. Examine and interpret the cross validation results. How do they vary in terms of time? Is the performance meaningfully different or just a little?
6. Try varying the cross validation parameters (eg the number of folds and/or type of cross validation). Does this change your conclusions?


```{tip}
this is best for regression or classification, but if you use clustering
use the `scoring` parameter to pass better metrics than the default
of the score method.
```

```{hint}
Assignment 11 will be to optimize two models and then compare two models on the same task
```

```{admonition} Thinking Ahead
What other tradeoffs might you want to make in choosing a model?
How could you present these results using your EDA skills?
```
