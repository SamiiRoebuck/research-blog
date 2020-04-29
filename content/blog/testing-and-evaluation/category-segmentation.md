---
title: 'Category update: Kitchenwares'
date: 2020-3-25 16:11:03
category: 'testing and evaluation'
---

From the evaluation of the last iteration of the model
([post can be viewed here](https://blog.samroebuck.dev/testing-and-evaluation/current-model/)) and testing of the app, I have determined that the accuracy of the kitchenwares catergory (originally called homewares, that has been changed because kitchenwares was more representative) is too low to be acceptable in production.

### Problem

Upon reviewing the dataset from which this category was trained upon and the confusion matrix from the associated model, I have determined that the reason for the low level of accuracy in this category is that there is too much variation in the objects labelled as kitchenware, the category contains a broad range of things from pans, to cutlery to cups etc. Because of this there is too much area for confusion within one single category to be sufficient.

This issue was noted as being a potential outcome when determining categories ([post can be viewed here](https://blog.samroebuck.dev/testing-and-evaluation/category-update/)).

### Solution

The fix to this problem was to segment this category into smaller categories so the dataset for each was more specific. Much like how the furniture prediction is achieved, the kitchenware response is created by creating and training smaller subcategories that once the prediction is given to the front-end logic of the app returns kitchenware as the prediction rather than the individual category.

This is beneficial not only because it increases the accuracy of the model response overall but it also hides some initial incorrect predicitions. This is because if the model incorrectly predicts one item within the kitchenwares subcategory as a different item in that subcategory, the response the user sees will still be correct as all items within the kitchenwares category are recycled in the same way. For instance, if the model predicts that something is a pan, the user will see the response 'It's kitchenware' and that it is recycled at a recycling centre, and if the model predicts it is crockery, the user will see the same response. This is the same technique that is used for the furniture subcategories as anything assigned as a bed or chair etc will give the user the same response.
