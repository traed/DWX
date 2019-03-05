# Docker Wordpress xDebug

A docker-compose template for setting up Wordpress, persistant storage with MariaDB and xDebug.

## Getting started
1. Make sure you have docker and docker-compose installed and up to date.
2. Clone the repo.
	- `git clone https://github.com/traed/dwx my-project && cd my-project && rm -rf .git`
3. Copy .env-example to a new file called .env and change the IP address to your local IP for xDebug to work.
	- `cp .env-example .env`
4. Build and run with docker-compose.
	- `docker-compose up -d`
5. (optional) If using Duplicator, log into the container and remove all files from /var/www/html and place the duplicator files there. Then go to /installer.php in the browser.