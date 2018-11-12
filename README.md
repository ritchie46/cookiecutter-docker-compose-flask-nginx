# Docker-compose Flask NGINX
This is a cookiecutter template for quickly deploying a Flask app with docker-compose. It is setup with NGINX as a 
reverse proxy to serve the static files underneath the *web/static* directory.

## requirements
* You'll need a [Docker](https://docs.docker.com/install/linux/docker-ce/ubuntu/) & [Docker-compose](https://docs.docker.com/compose/).
* Cookiecutter should be installed in a Python environment: `pip install cookiecutter`

## Start a new project

Clone the repository:

`$ git clone https://github.com/ritchie46/cookiecutter-docker-compose-flask-nginx.git`

Run cookiecutter to create a new project:

`$ cookiecutter cookiecutter-docker-compose-flask-nginx`

`$ cd <your-directory-name>`

Build the docker images and run the docker-compose service:

`$ docker-compose up`

## Validate it is up and running

`$ curl 127.0.0.1:80`

`> Hello World!`


## Teardown

Remove all the docker containers:

`$ docker-compose down`