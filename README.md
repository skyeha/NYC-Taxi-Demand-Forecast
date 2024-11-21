# New York City: Forecasting Monthly Taxi Demand
## Project Overview
This project is the first assignment of the subject Applied Data Sciece (MAST30034) at The University of Melboune. In this project, I decided to predict the monthly demand for taxi rides in New York City as well as exploring how other factors - socio-economic, weather - may affect such demands. Information on taxi rides were collected from NYC's Taxi & Limousine Commission. Additional data suchs as socio-economic and weather were found at U.S Beaurau of Labor Statistics and the US National Center for Environmental Information.

This project required applications of data cleaning such as removing null entries, entry with values that do not align with the data dictionary, and adopting a suitable method for outlier removal to discard a reasonable amount of entries. Geospatial analysis was performed to identify taxi trends and enhance understanding regarding which type of people are more likely to grab a taxi, and explore if geographical location plays a role in taxi demand.

Suitable machine learning models were employed for the tasks, namely Poisson Generalized Model and Random Forrest Regression. 

## Timeline
This project took 4-5 weeks to complete.

## Recreating The Project
To recreate this project:
* Clone this repository
* Create a folder called `data`.
* Inside `data/` directory, create 3 more folders, `data/raw`, `data/curated`, `data/landing`

After completing the initial setup, to run the pipeline, please visit the `notebooks` directory and run these notebook in the following order:
1. `1.raw_data_collection.ipynb`: This downloads the raw data from NYC TLC, NCEI, and  US BLS into the `data/raw` directory.
2. `2.1 trip_records_processing.ipynb` and `2.2 supplementary_data_processing.ipynb`: These notebook detail all preprocessing steps on all datasets and outputs them to the `data/curated` directory.
3. `3. data_analysis.ipynb`: This notebook is used to conduct analysis on the curated data.
4. `4.1 rfr_model.py` and `4.2 glm_model.py`: These notebook are used to run the fit, train, validate the model. After training, the models were use to predict demands and output the results to the `data/curated` directory.
5. `5. model_evaluation`: This notebook is used to plot graph, comparing predictions of 2 models with the ground truth
