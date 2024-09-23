# Gorkha Nepal Earthquake (2015): Exploratory Data Analysis and Classification

This project focuses on the 2015 Gorkha Nepal Earthquake, analyzing its impact using building and geographical data. The objective is to explore the data, perform feature engineering, and classify building damage levels, with a special focus on **geospatial embeddings**.


## Introduction
The 2015 Gorkha Nepal Earthquake caused significant damage to buildings and infrastructure. This project aims to classify the damage sustained by buildings based on factors like geographical location, building materials, building features, and buiding usage. A Random Forest classifier was used, enhanced by the integration of **geospatial embeddings** to improve classification performance.

## Dataset
The dataset includes detailed information about buildings, their geographical location, usage, and structural properties. Key columns include:
- **geo1**, **geo2**, **geo3**: Hierarchical geographical identifiers (region, sub-region, area)
- **age**: Age of the building
- **families_count**: Number of families residing
- **damage_grade**: Target variable indicating the level of building damage

You can find more about the data [here](https://www.drivendata.org/competitions/57/nepal-earthquake/page/134/).


## Project Workflow
1. **Data Preprocessing**: 
   - Cleaned and prepared the dataset by handling missing values, scaling numeric features, and encoding categorical variables.
2. **Exploratory Data Analysis (EDA)**: 
   - Visualized geographical distributions, damage patterns, and correlations between building features and damage.
3. **Feature Engineering**: 
   - Created geospatial embeddings to capture regional influences on building damage.
4. **Classification**: 
   - Used a Random Forest, Gradient boosting and ANN models to classify damage levels based on input features.

## Exploratory Data Analysis
EDA focused on understanding the distribution of damage across regions, the relationship between building age and damage, and identifying regions most prone to damage. Key visualizations included:
- Damage grade vs building age
- Damage distribution by region (geo1, geo2, geo3)
- Building material vs damage

## Geospatial Embeddings
Geospatial embeddings were created to encode geographical information. This allows the model to understand spatial dependencies between regions and buildings, capturing complex spatial patterns in earthquake damage.

Data is imbalanced and cost of predicting false positives and false negatives is high, so f1-score is choosen as an evolution metric.
