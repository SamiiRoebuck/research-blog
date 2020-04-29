---
title: 'In progress model response evaluation'
date: 2020-1-20 16:21:13
category: 'testing and evaluation'
---

_Current full data set count: 2510_

At this point, the image set from which the model is trained of mainly consists of clear images, with the subject central to the image with a plain background. This was purposeful done for the purpose of getting a functional version of the model working for the prototype and to see how consistent/correct the model could be made and whether it was possible to develop the level of functionality required for the project.

However, because of this the predications are less successful when the photo submitted has a messy background, is blurry or the image contains multiple items.

There are still categories I wish to add to the model: these include Tetrapaks, aerosols, and if time permitting, larger items such as furniture.

### Glass

_Current data set count: 730_

This is the most consistently correct category in terms of the predictions from the model, this is very clearly due to the fact that it has the largest subsection of the dataset attributed to it.

One very positive outcome of this section of the training is that under optimum conditions (plain background, clear image etc) the model is able to recognise items such as glass beakers/pint glasses as being within the glass category even though the majority of the glass dataset is of glass bottles. This is promising as it shows that the current dataset is sufficient for the machine learning API make successful predications without direct learning material.

This data set being significantly larger that many of the others is leading to items such as green plastic bottles being mistaken for green glass. From the point of the glass dataset, for this outcome to be minimised more variants of green and other coloured glass will need to be added for the model to be trained on.

### Plastic

_Current data set count: 686_

This category is also very consistent, however, as aforementioned there is an issue with green plastic bottles, such as Sprite bottles, being mistook for glass. This is likely due to the fact that a large amount of the images used to train the plastic category are clear bottles, film or white bottle such as milk bottles. There will need to be an increase in the amount of coloured plastic that is used to train the model in order to determine how well the app will be able to distinguish between these items.

### Cardboard

_Current data set count: 310_

This category performs surprisingly well considering the comparatively small subset of the data, consistently correctly predicting standard brown cardboard such as parcel packaging.

However, there are instances where there are varying incorrect predictions. This usually occurs when the cardboard is heavily printed on, such as cereal boxes, or appears to have a shiny coating under certain lighting conditions.

More variants of printed cardboard will be added to the dataset, along with images in varying lighting conditions in an attempt to prevent these incorrect predictions.

### Metal

_Current data set count: 292_

There is differing levels of success when predicting metals, when the item is something akin to a tin, bottle cap or can the successful predication level is quite high, especially considering the relatively low amount of image in the dataset assigned to this category. However where the predictions in this category fail are when it is tested on items such reusable metal water bottles or metal lunch boxes, broadly speaking items that are traditionally plastic.

Because of this there will need to be a much higher percentage of this section of the dataset committed to training the model on these items so that it can distinguish them from items that may be the same shape but are a different material.

Additionally, there are varying levels of success when the label is still attached to tin cans, in this case the model will occasionally predict that the item is paper. More images of tin cans with labels still attached will be added.

Metal being the smallest subsection of the dataset, this category needs a far amount more adding for consistently correct predictions.

### Paper

_Current data set count: 490_

The paper predictions are consistently correct, with the main exception being that it can occasionally be mistaken for cardboard if it's not plain paper.

This is a simple fix as it simply requires more variants of paper added to the dataset.
