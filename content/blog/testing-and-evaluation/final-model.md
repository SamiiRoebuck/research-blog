---
title: 'Completed Product - Retrospective'
date: 2020-5-08 10:01:20
category: 'testing and evaluation'
---

Upon completion of Kerbit, I have looked back on the pitch document and the improvement needed section of my prototype documentation and compared these to what I achieved with the completed version of Kerbit and dicuss whether I have achieved what I indended, if not why I think it was not achieved, and what I would have done differently if I was to conduct the development of this app again.

# Pitch Document points

## The original aim

- To help tackle the recycling contamination problems that Leeds has by making it easier to know where and how to recycle all kinds of items

Obviously there is not much way of knowing if the app has helped the recycling contamination with wide spread usage but I feel as though this aim has been met when considering the functionality that the app has. As when photos of items are taken the user is give the information of where and how to recycle the items.

## The original objectives

1. Have an extensive database of Leeds City Council recycling information and recycling centre locations

This objective did not end up being met due to a database not being deemed necessary within the development of the app. More can be read about why this change was made [here](https://blog.samroebuck.dev/testing-and-evaluation/change-in-db-requirements/) but in short it was determined that a database was no longer necessary due to an open source GeoJSON dataset being available for this purpose that could be loaded directly into the app.

2. Design an interface the will stay consistent across devices to ensure coherent user experience.

I feel as though this objective has been sucessfully met, especially when veiwing the app on iOS and Android there is very little variant in the app stylings and no variation in function.

3. Create an image classification model that runs at a good speed with accurate prediction

The acheivement of the objective is more vague than the others. The model speed and accuracy is something that I wish could be better but due to the model being built in a 'best trade off' way to balance out the speed and accuracy there is always going to be some loss in both of these areas to benefit the other area.

The prediction speed and accuracy is good when images are clear and uncluttered but there is some latency and inaccuracy when more complex images are used. However, considering how long these model take to train in industry to be at the accuracy level of commericial image classification models I am overall happy with it's performance.

4. Set up a Progressice Web App to use native camera functions

This objective has definately been met as the camera is accessible from the app on all supported devices.

# Prototype improvement points

1. Continuting to add images to the dataset to improve classification accuracy

In the prototype improvement section I acknowledged that it is unlikely to be 100% accuracy 100% of the time but that more images would be added to continue the training and attemping to improve the accuracy. I feel as though the accuracy of the categories has improved from the protoype although the same considerations mentioned in objective 3.

2. Increasing dataset size

I stated that I intended to have 1000 images in each category to make the model as accuracte as possible. However I didn't account of the decrease in speed that the larger models would cause or the difficulty or time needed to finding 1000 images that are good enough to be used in model training. Because of this the actual image datasets vary from 500-1000 in different categories as instead of forcing the 1000 images I decided to stop when that category was deemed accurate enough.

3. Prediction speed

In the prototype documentation I stated that I endevoured to improve the prediction speed by optimizing the app and the model. While the speed of the prediction did not greatly improve, due to a larger model being needed to add more categories, I did take all possible steps to optimize the app to save on speed where possible with the production bundle of the app being around 350kb.

## What would I do differently

The process of developing this app has given me many insights and has taught me many things which I would apply to if I would build something like this again.

Starting this I had very minimal knowledge of how training machine learning models work and thus went into this project with far too high of an expectation of how accurate I wanted the model to be. If I was to attempt something like this again I would go into the project with a much better overview of how the process works and what the best steps are to take. For instance, looking back I would have rather determined the full list of categories before starting any model training as everytime a new category is added the old model can not be retrained on top of due to the base dataset beign different. Because of this, I feel as though too much time was wasted training models from the ground up rather than retraining as due to the prototype model having different categories than the intended final model there was reduced possibilities for retraining.

Additionally, if I was to conduct the development of an app again I would spend more time in the initial stages on researching variations in API support and avaliability across different devices as I feel as though I lost some time in development and increased the time needed for testing by originally aiming to use features that I didn't know weren't widely supported, such as being able to use the flash.

## Conclusion

I do wish that the model predictions were faster and had higher levels of accuracy but considering I went into this with also zero knowledge of how machine learning works I am happy with what I was able to acheive in a relatively short amount of time. I am very happy with the look and feel of the app, I think I have done really well in building with and implementing modern web development technqiues. Overall I am happy with the app, with what I have achieved and I will proudly be displaying the project on my portfolio.
