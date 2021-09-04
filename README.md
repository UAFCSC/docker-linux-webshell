### CSC Linux Env

This project requires docker-compose and docker to build.  
Serves a web shell behind an nginx proxy.

## Running
`sudo docker-compose up -d`  
vist `webshell.localhost`  
ssh to other containers by docker names.  
`ssh root@ubuntu-0` 
password is csc for all containers

## Container list

- ubuntu-0
- ubuntu-1
- ubuntu-2
- ubuntu-3
- ubuntu-4
- ubuntu-5
- ubuntu-6

## TODO


Add basic auth to reverse proxy
