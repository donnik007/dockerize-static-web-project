# dockerize-staticwebproject
Example to dockerize a static web project. This is a simple todo application developed with jquery.

The idea here is to serve this static app using Nginx. Traditionally, we copy the project contents in a server, install nginx and configure nginx to serve the project content.

In docker approach, a docker container is created with nginx installed, configured and project contents copied. The applicaiton should start running when you just run "docker run"

Docker file cotains following steps

1. include nginx
2. replace nginx default configuration with local configuration files
3. copy project contents 
4. run nginx

Building docker container

docker build .

Running docker container
docker run -p 3000:80 -d --name=todo <<imageid>>

goto localhost:3000, and see your app in action



