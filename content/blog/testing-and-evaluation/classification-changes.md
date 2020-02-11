---
title: 'Classification category changes'
date: 2019-5-31 16:21:13
category: 'testing and evaluation'
---

From the dataset gathering and training of the model for the prototype it is becoming apparent that training a model to not only recognise the material of an item but also the item type, for instance, the item being plastic and also being a bottle, may be not only somewhat out of reach in the scope and timing of this project, but also has the potential to make the model too large to viably be part of a PWA in which the model will need to be cached on a users device to work offline.

In terms of the originally envisioned classifications, these are likely to be too large for this project as to have a consistently correct category, the dataset for that single category ideally needs to be upwards of 1000 images. Thus if the categories are broadly material based, i.e. plastic, metal, cardboard, paper, glass, furniture, tetrapak the total number of images needed is comparatively small when compared to if the categories were by type as well, i.e. plastic bottle, plastic film, plastic packaging, glass bottle, glass cup, brown cardboard, chair, table, grease paper e.t.c.

The incredibility high number of images needed for the originally intended model categories would also greatly impact the speed taken to return the prediction and overall speed of the PWA when running on an offline device. This is due to the model itself getting larger the more categories that are added to the model.

Because of these issues, for the foreseeable future the model with be trained on broader material based categories with the potential for a limited amount of common item based categories being added if the size of the app permits it and if there is sufficient development time to allow it.
