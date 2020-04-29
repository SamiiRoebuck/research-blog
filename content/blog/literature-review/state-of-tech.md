---
title: 'The state of tech: AI and Machine Learning'
date: 2020-01-05 11:21:13
category: 'literature review'
---

Artificial intelligence is a term for a broad range of tools used for making computers and computer systems behave intelligently, this includes a wide range of things like voice assistants and recommendations systems. (Bowne-Anderson, 2020). Machine learning comes under the category of AI tools as it is a 'branch of artificial intelligence which deals with the design and the development of algorithms and techniques to help machines learn' (Mellouk and Chebira, 2009, p.vii) from exisiting data and then have the ability to apply the learning to new data. These technologies have 'revolutionalized the world as we know it in the past decade' (Stewart, 2019) due to the rapid increase in the quanitities of data available caused by the increasing digitisation of daily life and the 'rapid development of processor power and computer parallelization' (Stewart, 2019) has made the usage of huge amounts of data far easier than every before. With the rise of machine learning related sevices and ubiquitous computing it is important to research and understand the industry use, and state of these technologies to gain background knowledge of the standard to which these tools are created.

### Industry usage

Within the industry there has been a 'strong evolution of Enterprise-grade ML platform solutions (Fernandez, 2020) including many from the media industries such as Facebook's FBLearning and Twitter's Cortex as well as an increase in machine learning services and vendors, such as Google AutoML, Microsoft Azure ML and IBM Watson. As well as a fast rise in the adoption of ai and machine learning across research and development across all industry departments (Columbus, 2019), the increasing value of the machine learning market, which is expected to expand rapidly and globally (Analytics Insight, 2019), is diverting machine learning and artificial intelligence tools in daily life from usage in healthcare for both patient care and administrative processes (Davenport and Kalakota, 2019), to self driving vechines, to cybersecurity, and digital assistants.

### State of Machine Learning models

The performance of machine learning models vary based on the algorithm used to train the model, and the model type. While the nuances of machine learning algorithms are out of the scope of this project due to the indended training of Kerbit being done using machine learning vendors, like the aforementioned, Google AutoML and IBM Watson, which do not make their base algorithms are accessible for comparison, the factors that can impact the accuracy of the intended model is still vital to consider to be able to set a baseline for performance of the indended system.

When considering how good these models can there are a number of things that have to be considered. It is alway important to take into account that 'achieving 100% accurarcy is never possible' (Tryo Labs, 2013a) due to algorithmic faults as well as human error in initial classification. Additionally, it important to consider the business importance and how that will impact what is deemed a well performing model (Tryo Labs, 2013b), as the baseline accuracy of a model used in medical treatment needs to be far more accurate that an a sentiment anaylsis model used on tweets. Finally, the type of classification is also important because this affects the accuracy regardless of how good the dataset is, for instance, a binary classification system, one that has only 2 labels, will always have a better accuracy performance than multicategory classification system as with more categories there is more potential for confusion.

The specific type of model that Kerbit will be implementing is an multi-category image classification model, it will be trained on various categories of images with the goal of identitifying what the image represents (Tensorflow, 2020) by returing a probability score for each category. All of the aformentioned considerations will impact the accuracy and performance of the indended model and therefore the likilhood of which Kerbit will give a user the correct answer.

While there is no overarching baseline percentage used to deem whether a model is sufficiently accurate, these factors can allow an estimation of Kerbit's baseline accuracy before any training is done. From knowing that the model accuracy is likely to be affected by human error in classification, will be multicategory so will inheriently by less accurate, that it is impossible to reach 100% accuracy and when considering the business importance of the accuracy of the model, it is felt that a baseline accuracy of 80% will be a good aim to reach for within Kerbit's development.

## References

Bowne-Andersone, H. 2020. _The Difference between AI and Machine Learning_. [Online]. [Accessed 26 March 2020]. Available from: https://www.datacamp.com/community/blog/ai-and-ml?utm_source=adwords_ppc&utm_campaignid=9942305733&utm_adgroupid=100189364546&utm_device=c&utm_keyword=&utm_matchtype=b&utm_network=g&utm_adpostion=&utm_creative=229765585183&utm_targetid=dsa-929501846124&utm_loc_interest_ms=&utm_loc_physical_ms=1006864&gclid=CjwKCAjwqJ_1BRBZEiwAv73uwH-5q0OTzCkZRFJIfFZoKAeGQjt5KGliL1Hrd5-7_bhyuMjgnADcehoCNBkQAvD_BwE

Mellouk, A., and Chebira, A. 2009. Preface. In: Mellouk, A., and Chebira, A. 2009. ed(s). _Machine Learning_. [No place of publication]: IntechOpen, p.vii - x.

Stewart, M. 2019. _The Limitations of Machine Learning_. [Online]. [Accessed 26 March 2020]. Avaliable from: https://towardsdatascience.com/the-limitations-of-machine-learning-a00e0c3040c6

Tensorflow, 2020. _Image classification_. [Online]. [Accessed 28 March 2020]. Avaliable from: https://www.tensorflow.org/lite/models/image_classification/overview#what_is_image_classification

Fernandex, E. 2020. _State of the Machine Learning and AI Industry_. [Online]. [Accessed 28 March 2020]. Avaliable from: https://towardsdatascience.com/state-of-the-machine-learning-ai-industry-9bb477f840c8

Columbus, L. 2019. _State of AI and Machine Learning in 2019_. [Online]. [Accessed 28 March 2020]. Avaliable from: https://www.forbes.com/sites/louiscolumbus/2019/09/08/state-of-ai-and-machine-learning-in-2019/#1624335e1a8d

Analytics Insight. 2019. _The State of Machine Learning in 2019_. [Online]. [Accessed 28 March 2020]. Avaliable from: https://www.analyticsinsight.net/the-state-of-machine-learning-in-2019/

Davenport, T., and Kalakota, R. 2019. The Potential for Artificial intelligence in healthcare. _Future Healthcare Journal_. **6**(2), pp.94-98.

Tryo Labs, 2013a. _Machine Learning Basics_. [Online]. [Accessed 29 March 2020]. Avaliable from: https://tryolabs.com/blog/machine-learning-basics-every-manager-should-know/

Tryo Labs, 2013b. _Why accuracy alone is a bad measure for classification tasks, and wwhat we can do about it_. [Online]. [Accessed 29 March 2020]. Avaliable from: https://tryolabs.com/blog/2013/03/25/why-accuracy-alone-bad-measure-classification-tasks-and-what-we-can-do-about-it/
