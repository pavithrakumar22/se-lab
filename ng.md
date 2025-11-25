Open docker

Open powshell

docker pull jasonrivers/nagios: latest

docker run --name nagiosdemo -p 8888:80 jasonrivers/nagios: latest

go to browser: localhost:8888

nagiosadmin
nagios

go to hosts

click localhost

open another powshell

docker ps

docker stop nagiosdemo

docker rm nagiosdemo

