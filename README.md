# Personal thermal comfort models using digital twins: Preference prediction with BIM-extracted spatial-temporal proximity data from Build2Vec

This repository includes some of the code needed to reproduce the work in a preprint submitted to Building and Environment.

## Abstract

Conventional thermal preference prediction in buildings has limitations due to the difficulty in capturing all environmental and personal factors. New model features can improve the ability of a machine learning model to classify a person's thermal preference. The spatial context of a building can provide information to models about the windows, walls, heating and cooling sources, air diffusers, and other factors that create micro-environments that influence thermal comfort. It is impractical to position sensors at a high enough resolution to capture all conditions due to spatial heterogeneity. This research aims to build upon an existing vector-based spatial model, called Build2Vec, for predicting spatial-temporal occupants' indoor environmental preferences. Build2Vec utilizes the spatial data from the Building Information Model (BIM) and indoor localization in a real-world setting. This framework uses longitudinal intensive thermal comfort subjective feedback from smart watch-based ecological momentary assessments (EMA). The aggregation of these data is combined into a _graph network structure_ (i.e., objects and relations) and used as input for a Graph Neural Network (GNN) model to predict occupant thermal preference. The results of a test implementation show 14-28\% accuracy improvement over a set of baselines that use conventional thermal preference prediction input variables.

## Requirements

```
build2vec
networkx
pandas
geopandas
scikit-learn
```

## Reproducibility

1. Goto `./code` folder
2. install requirements `pip3 install -r requirements.txt`
3. open the `code.ipynb` notebook
4. run the code

## example output

Spatial similarity between different cells

![ezgif-4-73470bfbefdf](https://user-images.githubusercontent.com/6969514/138804697-6e3cdebe-5ec1-4518-9637-6a07ae8c40a5.gif)
