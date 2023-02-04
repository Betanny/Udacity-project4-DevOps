[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Betanny/project4/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Betanny/project4/tree/main)
## Project Overview
CONTAINERISATION
operationalizationof Machine Learning Microservice API

HOUSING PRICE PREDICTION
Data source : https://www.kaggle.com/c/boston-housing


Preriquisites:
    - Docker hub account
    - CircleCI account
    - You should have Python 3.7 available in your host.
    
    

PROPOSED KUBERNETES STEPS
- Testing the project code
- Setting up docker
- Configuring docker
- Create a flask app in a container
- Run it via kubectl
- Deploy and configure kubernetes cluster
- Verify and load auto-scaling
 



    

Steps
- create project
    - Complete Dockerfile
    - App
    - Pickled model
- Build and test the project
- Push docker image to DockerHub
- Predict via the container in cloud 9
- Integrate it to circleCi


RUNNING PYTHON SCRIPTS
- python3 -m pip install --user virtualenv
- source .devops/bin/activate
- make install // install the neccessary dependencies
- 

Runnng the app:
 standalone -    python app.py
 Docker -    ./run_docker.sh
 Kubernetes -   ./run_kubernetes.sh


Summary of files
- .circleci - contains the configuration file for CicleCi in yaml format
- model_data - Data used in the project
- output_txt_files - contains the output of the kuberenetes and docker execution
- dockerfile - configuration for docker
- makefile - contains instructions on environment setup and lint tests
- cmd.txt - history of some the commands used
- cmd4.txt - history of some the commands used
- resize.sh - commands for resizing the volume as needed
- run_kubernetes.sh - running kubernetes
- upload_docker.sh - uploading the docker image to docker hub
- run_docker.sh - building the docker image