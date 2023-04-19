
# Assignment 12: Fake News

## Quick Facts
- [accept the assignment](https://classroom.github.com/a/QRTv4_g_)
_due date:2023-04-26__
<!-- - First feedback: {{ early }}
__Final due date: {{ date }}__ -->


## Related notes

- [](../notes/2023-04-18)
- [](../notes/2023-04-20)

## Assessment

Eligible skills: (links to checklists)
- **first chance** representation [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#representation-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#representation-level2) remember this is optional
- **first chance** workflow [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#workflow-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#workflow-level2) psuedo code and explanation is enough for this
- compare [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#compare-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#compare-level2)
- optimization [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#optimization-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#optimization-level2)
- clustering [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#clustering-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#clustering-level2)
- classification [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#classification-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#classification-level2)
- evaluate (must use extra metrics to earn this here) [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#evaluate-level2)
- summarize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#summarize-level2)
- visualize [1](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level1) and [2](https://rhodyprog4ds.github.io/BrownFall22/syllabus/achievements.html#visualize-level2)


## Instructions

Use the dataset in the assignment template repo to answer the following questions.

1. Is the text or the title of an article more predictive of whether it is real or fake?
1. Are titles of real or fake news more similar to one another?

The data includes variables:
- ‘text’: contents of an article
- ‘label’: whether it is real or fake news
- 'title': title of the article

Include narrative around the code required to answer these and interpret the results to give an actual answer. 
- Provide context on your answer and consider how strong it is based on what differences you can have in how you represent the data and how that might impact your model performance. 
- Consider if the analysis you have done is enough evidence answer the question from the analysis you have completed or could something else chang the answer. 
- Use summary statistics and visualizations appropriately in order to explain your results.

```{hint}
The data set contains a large number of articles (takes a long time to train), you can downsample this to something like a 1,000 articles or so in order to speed up training and evaluation (hint: use shuffle).

```
