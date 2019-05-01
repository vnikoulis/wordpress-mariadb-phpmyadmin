![Image of docker, wp and phpmyadmin](https://i.imgur.com/kjOuf9a.jpg)
# Wordpress, MariDB & phpMyAdmin Docker Compose
This project allows you to develop with Wordpress using Docker and Docker compose

## Configuration
You can edit the name, root password and the user of the database by simply editing the `docker-compose.yml` file.

## Installation
Clone this repository into a folder. Then you have to create a network with the command:
```
docker network create main_net
```
I have named my network `main_net` but you can name your network as you like but you have to edit the
```
networks: 
    - main_net
```
tag in the `docker-compose.yml` file.
The you `cd` to the folder that the `docker-compose.yml` file is saved and run:
```
docker-compose up
```
You are now ready to use Wordpress and phpMyAdnin by visiting `localhost:8080` for phpMyAdmin and `localhost` for Wordpress.
