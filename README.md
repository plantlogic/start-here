[![Issues](https://img.shields.io/github/issues/plantlogic/start-here.svg?style=flat)](https://github.com/plantlogic/start-here/issues) [![License](https://img.shields.io/github/license/plantlogic/start-here.svg?style=flat)](https://github.com/plantlogic/start-here/blob/master/LICENSE) [![pullreminders](https://pullreminders.com/badge.svg)](https://pullreminders.com?ref=badge)
# 🌱 PlantLogic | Start Here

## **Introduction**

PlantLogic is a web application developed in collaboration with Merrill Farms, a Salinas, California based vegetable grower and agricultural employer, and serves to connect all parties involved in the process of growing agriculture while managing relevant data used in the process. The project aims to assist, and potentially replace, the current system of record keeping which involves noting data down on cards while at fields or farms and later re-recording these over to a separate digital system. 

Recording information about a single commodity can involve several dozen pieces of data: variety of the commodity, irrigation dates, hoeing and thinning dates, chemicals and fertilizers, ranch names, lot numbers, which group or person did what job, etc..; By using a more comprehensive system for record keeping, there is improved data consistency and accuracy as well as better data organization. In addition, with growing complexity around agriculture regulations, there is also a desire to add compliance checks and an alert system in the future to allow record keepers to comply with regulations more easily.

</br>

## **Technology Overview**

PlantLogic is composed of 3 Dockerized microservices:

| Service  | Status |
|----------|--------|
| [Frontend](https://github.com/plantlogic/frontend/) | [![Build Status](https://travis-ci.org/plantlogic/frontend.svg?branch=master)](https://travis-ci.org/plantlogic/frontend) [![Issues](https://img.shields.io/github/issues/plantlogic/frontend.svg?style=flat)](https://github.com/plantlogic/frontend/issues) [![Docker Pulls](https://img.shields.io/docker/pulls/projectnull4/plantlogic-frontend.svg?style=flat)](https://hub.docker.com/r/projectnull4/plantlogic-frontend)           |
| [User Service](https://github.com/plantlogic/user-service/) | [![Build Status](https://travis-ci.org/plantlogic/user-service.svg?branch=master)](https://travis-ci.org/plantlogic/user-service) [![Issues](https://img.shields.io/github/issues/plantlogic/user-service.svg?style=flat)](https://github.com/plantlogic/user-service/issues) [![Docker Pulls](https://img.shields.io/docker/pulls/plantlogic/user-service.svg?style=flat)](https://hub.docker.com/r/plantlogic/user-service) |
| [Data Service](https://github.com/plantlogic/data-service/) | [![Build Status](https://travis-ci.org/plantlogic/data-service.svg?branch=master)](https://travis-ci.org/plantlogic/data-service) [![Issues](https://img.shields.io/github/issues/plantlogic/data-service.svg?style=flat)](https://github.com/plantlogic/data-service/issues) [![Docker Pulls](https://img.shields.io/docker/pulls/plantlogic/data-service.svg?style=flat)](https://hub.docker.com/r/plantlogic/data-service) |

The Frontend service is built using the Angular web application framework and, as the name suggest, serves the front-end to the client as a single page application which utilizes Angular routing. The User and Data services are built using Java Spring Boot and manage MongoDB database operations and access for user data and non-user data respectively.

This repo is where setup info with Docker Compose and NGINX (or another gateway) will be stored.

</br>

## **Installation**
To setup, [clone](x-github-client://openRepo/https://github.com/plantlogic/start-here) or [download](https://github.com/plantlogic/start-here/archive/master.zip) this repo. Then, copy the `docker-compose.example.yml` file to `docker-compose.yml` and edit the appropriate environment variables for the `frontend`, `userservice`, and `dataservice` containers. More detail on each of these environment variables can be found in the README of the repo for each service (see the table above).

![Example Homepage](https://user-images.githubusercontent.com/420820/59152014-6409d380-89f1-11e9-8e0b-6d276dfb3bd2.png)
Example Homepage