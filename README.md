# mds_fernandes_alexandre_2021_secu

## Introduction
:school: This Project secured app is a REST API, an authentification API, mongoDB and a reverse proxy service with nginx 

## **🧱 Structure**

In folder auth-api, products-api, nginx and client we will find a Dockerfile to build the image.
In main repository we will find a docker-compose.yml to set containers launching:

> ./docker-compose.yml

<br/>

## **⚙️ Setup Composing**

Dockerfile content:

> **FROM**: Use a lighter version of Node as a parent image
>
> **WORKDIR**: Set the working directory
>
> **COPY**: Copy the current directory contents into the container at /api
>
> **RUN**: install dependencies
>
> **EXPOSE**: Make port XXXX available to the world outside this container
>
> **CMD**: Run the app when the container launches

In docker-compose.yml:

_we will find there the version and the services of deployment_

<br/>

## **:rocket: Install & Deployment**

> :\$ git clone https://https://github.com/Yowks/mds_fernandes_alexandre_2021_secu.git

Use docker:

> :\$ **docker-compose up --build** or **docker-compose up -d --build**
>
> _Shutdown if necessary: :\$ docker-compose down_
> 
> Basic for use cluster: 
> :\$ **docker-compose up**

<br/>



:memo: Note

Connection db `mongodb://mongodb:27017/products

Auth-api port `https://localhost:3001` <br>
Products-api port `https://localhost:3002`
Client access `https://localhost:3000`