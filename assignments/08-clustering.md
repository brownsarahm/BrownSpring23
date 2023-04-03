---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/rzuWo1_-)
  date : 2023-03-29 
---
# Assignment 8: Clustering

 [accept the assignment](https://classroom.github.com/a/rzuWo1_-)
__Due: 2023-03-29__

## Evaluation

Eligible skills: (links to checklists)
- **first chance** clustering [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#clustering-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#clustering-level2)
- evaluate [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level2)
- python [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#python-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#python-level2)
- summarize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level2)
- visualize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level2)

_for some of these you will need to add analysis that is not described in the instructions below, but is related to this and that skill_

## Related notes

- [](../notes/2023-03-21)
- [](../notes/2022-03-23)



## Instructions

Use the same dataset you used for assignment 7, unless there was a problem. If you skipped assignment 7, choose a dataset well suited for classification.

1. Describe what question you would be asking in applying clustering to this dataset. What does it mean if clustering does not work well? 
2. Apply Kmeans using the known, correct number of clusters, $K$.
1.  Evaluate how well clustering worked on the data:

    - using a true clustering metric and
    - using visualization and
    - using a clustering metric that uses the ground truth labels
2. Include a discussion of your results that addresses the following:

    - describes what the clustering means
    - what the metrics show
    - Does this clustering work better or worse than expected based on the classification performance (if you didn't complete assignment 7, also apply a classifier)
3. Repeat your analysis using a 2 different numbers (1 higher, one lower) of clusters:

    - can you interpret the new clusters?
    - how do they relate to the original clusters? are they completely different, did one split?
    - is there a reasonable explanation for more clusters than there are classes in this dataset?
