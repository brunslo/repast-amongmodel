# Repast AMONG Model
## Overview
This project provides a Docker Compose script to allow both the AMONG model front- and backend components to be run locally without requiring any development tools.

## Usage
To build this you will need a local installation of git and Docker. First, clone this repository and initalise the submodules:
```
git clone --recurse-submodules https://github.com/brunslo/repast-amongmodel
```
Next you need to run Docker Compose to build and bring the various images up:
```
docker-compose up --build
```
That's it! It will take a while to build the images the first time, as the code for each sub-project has to be compiled and their dependencies have to be downloaded. Docker will cache these steps on subsequent runs which will dramatically speed things up.