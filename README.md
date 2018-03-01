# Docker Wordpress Sass xDebug

A docker-compose template for setting up Wordpress, persistant storage with MariaDB as well as Sass and xDebug.

To get started:
0. Make sure you have docker and docker-compose installed and up to date.
1. Clone the repo.
2. Open the .env file and change the placeholder to your local IP for xDebug to work.
3. Build and run with docker-compose.
4. If you change theme, update the volumes for Sass in the docker-compose file and rebuild.