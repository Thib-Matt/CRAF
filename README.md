# COVID Relevant Articles Finder

## Project Overview

This project is an answer to the call to action from the [COVID-19 Open Research Dataset Challenge (CORD-19)](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge) to leverage our expertise to help the medical community in the fight against coronarivuses.

We created a smart search engine that suggests relevant academic articles related to coronavirus based on user's request specific request.

This could help to generate new insights among over 400k articles about COVID-19, SARS-CoV-2, and related coronaviruses.

## Steps of the project

- data cleaning and preprocessing: refine and vectorize the abstracts to make them usable
- topic modelling: use the LDA (Latent Dirichlet allocation) to generate labels for the articles
- productionizing: build a Flask API and graphical user interface (web-app)
- deployment/DevOps: dockerize the whole solution

The scripts to prepare the model can be found in the [modelling](https://github.com/Thibault-Mattera/COVID-Relevant_Articles-Finder/tree/master/modelling) folder.

## How to use the web app

![](/images/covid-app-demo.gif)

Clone the github repository and run the following Docker commands.

docker-compose build

docker-compose up

Access to the web-app on your local server:

http://localhost:8080/

Stop the containers:

docker-compose stop
