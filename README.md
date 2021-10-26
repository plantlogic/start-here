[![Issues](https://img.shields.io/github/issues/plantlogic/start-here.svg?style=flat)](https://github.com/plantlogic/start-here/issues) [![License](https://img.shields.io/github/license/plantlogic/start-here.svg?style=flat)](https://github.com/plantlogic/start-here/blob/master/LICENSE) [![pullreminders](https://pullreminders.com/badge.svg)](https://pullreminders.com?ref=badge)
# 🌱 PlantLogic | Start Here

| Service  | Status |
|----------|--------|
| [Frontend](https://github.com/plantlogic/frontend/) | [![Build Status](https://travis-ci.org/plantlogic/frontend.svg?branch=master)](https://travis-ci.org/plantlogic/frontend) [![Issues](https://img.shields.io/github/issues/plantlogic/frontend.svg?style=flat)](https://github.com/plantlogic/frontend/issues) [![Docker Pulls](https://img.shields.io/docker/pulls/projectnull4/plantlogic-frontend.svg?style=flat)](https://hub.docker.com/r/projectnull4/plantlogic-frontend)           |
| [User Service](https://github.com/plantlogic/user-service/) | [![Build Status](https://travis-ci.org/plantlogic/user-service.svg?branch=master)](https://travis-ci.org/plantlogic/user-service) [![Issues](https://img.shields.io/github/issues/plantlogic/user-service.svg?style=flat)](https://github.com/plantlogic/user-service/issues) [![Docker Pulls](https://img.shields.io/docker/pulls/plantlogic/user-service.svg?style=flat)](https://hub.docker.com/r/plantlogic/user-service) |
| [Data Service](https://github.com/plantlogic/data-service/) | [![Build Status](https://travis-ci.org/plantlogic/data-service.svg?branch=master)](https://travis-ci.org/plantlogic/data-service) [![Issues](https://img.shields.io/github/issues/plantlogic/data-service.svg?style=flat)](https://github.com/plantlogic/data-service/issues) [![Docker Pulls](https://img.shields.io/docker/pulls/plantlogic/data-service.svg?style=flat)](https://hub.docker.com/r/plantlogic/data-service) |

This repo is where setup info with Docker Compose and NGINX (or another gateway) will be stored. Part of our CSUMB Spring 2019 capstone project developed in collaboration with Merrill Farms.

## Screenshots
![Example Homepage](https://user-images.githubusercontent.com/420820/59152014-6409d380-89f1-11e9-8e0b-6d276dfb3bd2.png)
Example Homepage

## Installation
To setup, [clone](x-github-client://openRepo/https://github.com/plantlogic/start-here) or [download](https://github.com/plantlogic/start-here/archive/master.zip) this repo. Then, copy the `docker-compose.example.yml` file to `docker-compose.yml` and edit the appropriate environment variables for the `frontend`, `userservice`, and `dataservice` containers. More detail on each of these environment variables can be found in the README of the repo for each service (see the table above).
