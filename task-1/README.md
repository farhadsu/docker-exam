Dockerfile builds a Docker image that uses NGINX, but replaces the default index.html
docker-compose.yml file configures the NGINX service to run on port 9090 of your local machine


1.Place the index.html, Dockerfile, and docker-compose.yml files in the same directory.
2.Open a terminal and navigate to the directory containing these files.
3.Run the following command to start the NGINX container using Docker Compose

docker-compose up --build 

build completes, you can visit http://localhost:9090 in your browser 