# Docker Wordpress xDebug

A docker-compose template for setting up Wordpress, persistant storage with MariaDB and xDebug.

To get started:
0. Make sure you have docker and docker-compose installed and up to date.
1. Clone the repo.
2. Copy .env-example to a new file called .env and change the IP address to your local IP for xDebug to work.
3. Build and run with docker-compose.
4. (optional) If using Duplicator, log into the container and remove all files from /var/www/html and place the duplicator files there. Then go to /installer.php in the browser.