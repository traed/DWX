# Docker Wordpress Sass xDebug

A docker-compose template for setting up Wordpress, persistant storage with MariaDB as well as Sass and xDebug.

To get started:
0. Make sure you have docker and docker-compose installed and up to date.
1. Clone the repo.
2. Copy .env-example to a new file called .env and change the IP address to your local IP for xDebug to work.
3. Build and run with docker-compose.
4. (optional) If using Duplicator, remove all files that get generated in the web directory and place the duplicator files there. Then to to /installer.php in the browser.

If you change theme, update the volumes for Sass in the docker-compose file and rebuild.