[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/Yi0Zbe2y)
# MAST30034 Project 1 README.md
- Name: Do Nhat Anh Ha
- Student ID: 1194034

**Research Goal:** Predicting monthly taxi demands using weather, socio-economic data and season effects.

**Timeline:** The timeline for the research area is  March 2023 - May 2024. The models were train using data from March 2023 to Febuary 2024 and were test using data from March 2024 to May 2024

**Model used:** *Random Forest Regression* and *Generalised Linear Model*

To run the pipeline, please visit the `notebooks` directory and run the files in order:
1. `1.raw_data_collection.ipynb`: This downloads the raw data from NYC TLC, NCEI, and  US BLS into the `data/raw` directory.
2. `2.1 trip_records_processing.ipynb` and `2.2 supplementary_data_processing.ipynb`: These notebook detail all preprocessing steps on all datasets and outputs them to the `data/curated` directory.
3. `3. data_analysis.ipynb`: This notebook is used to conduct analysis on the curated data.
4. `4.1 rfr_model.py` and `4.2 glm_model.py`: These notebook are used to run the fit, train, validate the model. After training, the models were use to predict demands and output the results to the `data/curated` directory.
5. `5. model_evaluation`: This notebook is used to plot graph, comparing predictions of 2 models with the ground truth