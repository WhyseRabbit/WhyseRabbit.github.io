---
layout: post
title: Learning Takes Time
subtitle: Metrics from Junyi Academy in China
gh-repo: whyserabbit
gh-badge: [star, fork, follow]
tags: [portfolio, lambda project]
comments: true
---

# Learning Takes Time

## Note for readers: The DataFrame being used is far too large to be hosted on GitHub. You can find the pertinent information on [Kaggle](https://www.kaggle.com/junyiacademy/learning-activity-public-dataset-by-junyi-academy). To solve this problem, I read in a 5% sample of the largest data, which equates to 810,866 observations.

#### Working Hypothesis: The more time and effort a student puts into learning a subject matter (in this case, math) makes it more likely for a student to learn that subject.

### **Project Considerations With Answers:**

- `Choose which observations you will use to train, validate, and test your model.`  
*The data was collected over the better part of two years; I split the data into sections using the time-date format. The training data is built from sample data in 2018; the validation data takes place between January and April, 2019, and the testing data resides in May until the end of the study.*  
- `Choose your target. Which column in your tabular dataset will you predict?`  
*`is_correct` will be my target. This is a binary classification of either `True` or `False`.*  
- `How is your target distributed?`  
  *70% `True`*  
  *~30% `False`*  
- `Choose your evaluation metric(s).`  
*Because the model is fairly balanced and Classification is needed, `accuracy` will be the evaluation metric.*
