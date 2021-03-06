---
title: 'Potential Category Change'
date: 2020-2-27 18:21:13
category: 'testing and evaluation'
---

After completing the prototype, experiencing the time needed to generate enough data to train a sufficient model, and taking time to re-sort over the different categories of recyclables on the Leeds.gov website, I have re-evaluated what categories are necessary for Kerbit to be a functional product as well as minimising the number of categories that need to be made.

### Categories for green bin recyclables

All these items are in the category of things that can be placed in the green bin that users will have at their home.

- Paper (covering post, packing paper, newspapers etc)
- Cardboard (covering packaging, cereal boxes etc)
- Metal (covering tin cans, aerosols, foil etc)
- Plastics (covering cartons/tetrapaks/food tubs etc)
- Plastic bags
  - This category is more specific than the others above as through testing I have determined that the model stuggles to make a connection between thin plastic bags and hard plastics like bottles. Because of this they have been separated into a different category.

### Categories of recycling centre recyclables

All these items are things that are either: broad categories of items that should be taken to recycling centres or charity shops or specific categories of items that are often mistaken for being able to be put in the green bin but actually have to be taken to a refuse centre or have to go into general waste.

_Broad categories_

- Glass (covering all bottles, jars, cups etc)
- Furniture\*
- Homewares\* (covering items like kitchen wear and home decorations)
- Electricals\* (covering items such as toasters, kettles, tv's)
- Textiles (covering items such as clothing, bedding, soft furnishing)

\* _These broad categories may need to be further segmented if there are high percentages of confusion during model training. However, the response given to the user will still be the broad category title_

With this new category set, I will create a survey to determine the recycling behaviour and knowledge from the demographic and determine if anymore catoregies need to be added or changed.
