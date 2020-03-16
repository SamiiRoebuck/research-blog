---
title: 'Database requirements Update'
date: 2020-3-16 18:21:13
category: 'testing and evaluation'
---

Initially, as part of the pitch document I anticipated that Kerbit would need a database for storing the locations of recycling centres which would then be used to query, once given the users location, and then display the nearest recycling centres or refuse points to user. This was accounted for in both the gantt chart for the time it would take to find all the data, set up and test and the costings of the app for the cost of hosting the database.

However, after doing some development with the Google Maps API I have discovered that you can load data directly into the map using GeoJSON, a map data specific form of JSON. A method that will be much more suitable for Kerbit as being a progressive web app any instance where having to fetch data can be removed will make the process of making the app work offline much simpler.

After determining that loading GeoJSON data would better suited to the app than having to query a database I researched into if there was any open datasets that already held any of this data. Luckily, a dataset released under a UK Open Government Licence contains the location data for all 'bring sites' in and around Leeds, which with a few formatting changes and the removal of unnecessary data this will be the perfect data to load into the map.

The dataset can be found [here](https://datamillnorth.org/dataset/bring-sites) along with the information regarding the licensing and attribution of the data.
