---
title: 'In progress: Model response evaluation'
date: 2019-5-31 16:21:13
category: 'testing and evaluation'
---

_Current full data set count: 2510_

At this point, the image set from which the model is trained of mainly consists of clear images, with the subject central to the image with a plain background. This was purposeful done for the purpose of getting a functional version of the model working for the prototype and to see how consistent/correct the model could be made and whether it was possible to develop the level of functionality required for the project.

However, because of this the predications are less successful when the photo submitted has a messy background, is blurry or the image contains multiple items

There are still categories I wish to add to the model: these include Tetrapaks, aerosols, and if time permitting, larger items such as furniture.

### Glass

_Current data set count: 730_

This is the most consistently correct category in terms of the predications from the model, this is very clearly due to the fact that it has the largest subsection of the dataset attributed to it.

One very positive outcome of this section of the training is that under optimum conditions (plain background, clear image etc) the model is able to recognise items such as glass beakers/pint glasses as being within the glass category even though the majority of the glass dataset is of glass bottles. This is promising as it shows that the current dataset is sufficient for the machine learning API make successful predications without direct learning material.

This data set being significantly larger that many of the others is leading to items such as green plastic bottles being mistaken for green glass. From the point of the glass dataset, for this outcome to be minimised more variants of green and other coloured glass will need to be added for the model to be trained on.

### Plastic

_Current data set count: 686_

This category is also very consistent, however, as aforementioned there is an issue with green plastic bottles, such as Sprite bottles, being mistook for glass. This is likely due to the fact that a large amount of the images used to train the plastic category are clear bottles, film or white bottle such as milk bottles. There will need to be an increase in the amount of coloured plastic that is used to train the model in order to determine how well the app will be able to distinguish between these items.

### Cardboard

_Current data set count: 310_

### Metal

_Current data set count: 292_

### Paper

_Current data set count: 490_
