Connect to ec2

Note: download the pem file in seperate folder

you will get ssh 

sudo apt update

sudo apt-get install docker.io

sudo apt install git

sudo apt install nano

//for index.html
open gitbash
push to github

in ubuntu

git clone

cd folder

create docker file

nano Dockerfile

FROM nginx:alpine
COPY ./usr/share/nginx/html

sudo docker build -t mywebapp .

sudo docker run -d -p 80:80 mywebapp

now go to browser with public ip using http


sudo docker stop container name



//for maven
Dockerfile

FROM tomcat:9-jdk11
COPY target/* .war /usr/local/tomcat/webapps/

sudo docker build -t mavenweb .

sudo docker run -d  -p 9090:8080 mavenweb
security
inbound rules







