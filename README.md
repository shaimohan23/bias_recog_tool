This repository contains the code for a political bias recognition tool.

The 4 python notebooks in this directory were developed in the order of 1. pre_process, 2. base_ml_models, 3. bert_model, and 4. llama_model

The pre-process notebook runs on the original csv data file that can be downloaded from https://www.kaggle.com/datasets/hadasu92/cnn-articles-after-basic-cleaning and put in the data folder.

The output of this notebook was then fed into gpt 4 through the chatGPT UI to label the dataset for further use and all the models start with the output of that (cnn_articles_large_trimmed_labeled_3.csv)

This file is then loaded into each of the other notebooks where the data is cleaned and then used to fine-tune each model for this task.  Graphs of some of the results are in the "graphs" folder within the data folder and were created separately from this code.

The config folder also has a json file that was used for my custom filter, and it can be modified to include more/different terms if needed.