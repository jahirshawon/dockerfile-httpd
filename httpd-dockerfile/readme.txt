## here we build httpd image from docker file and running container
##n.b here we need to create a index.html file on current directory

docker build -t web .

##check new images

docker images

##run container using build image

docker run --name webserver -dit  -p 8080:80 web

