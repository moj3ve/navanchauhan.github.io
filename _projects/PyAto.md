---
title: "PyAto"
excerpt: "A Python module for accessing Zomato's API"
sidebar:
  - title: "Languages Used"
    text: "Python3"
  - title: "License"
    text: "MIT"
---

### Initialisation
```
import PyAto
PyAto.setAPIKey("Your Key Here")
```
or
```
import PyAto as pyato
pyato.setAPIKey("Your Key Here")
```
### Functions

| Function | Required Values | Output |
|----------|-----------------|--------|
| getCategories | None | JSON |
| getCities | Name (String) | JSON |
| getCityID | Name (String) | Integer |
| getCollections | CityID (Integer) | JSON |
| getCuisines | CityID (Integer) | JSON |
| getGeocode | Latitude & Longitude | JSON |
| getEstabblishments | CityID | JSON |


