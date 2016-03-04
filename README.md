# Node server full flow exemple 

Exemple to integrate CI + auto-deployment on a remote server using docker

## Motivation

I wanted to try to have a hello-world projet for a node server that is easy to deploy.

I also wanted to see how I can integrate CI and auto-deployment

## Tags

Tag v1.0 "http-hello-world": Simple hello world http server (listening on port 80)

## Installation

If you want to have this server up

### Install docker + docker compose

1. Install docker 'wget -qO- https://get.docker.com/ | sh'
2. Set user in docker 'sudo usermod -aG docker $(whoami)'
3. Logout (necessary for the user to be set correctly in docker)
4. Install pip (necessary for docker-compose): 'sudo apt-get -y install python-pip'
5. Install docker-compose: 'sudo pip install docker-compose'


### Clone the repo

1. Clone this repo: 'git clone  https://github.com/PrincessMadMath/docker_full_flow_exemple.git'


### Run the server

1. Go in the repository eith the "docker-compose.yml" file
2.1 Start the server: 'docker-compose up'
2.2 Start the server in background: 'docker-compose up -d'


## Test

1. Install curl
2. Receive an hello world: 'curl localhost'


## Troubleshooting

### See the docker logs
### See the nginx logs
### Open the port on the server



## Useful Source

1. Install docker compose on ubuntu: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-14-04
2. Complete exemple with node, nginx and redis : http://anandmanisankar.com/posts/docker-container-nginx-node-redis-example/
3. nginx config file explained: https://www.digitalocean.com/community/tutorials/understanding-the-nginx-configuration-file-structure-and-configuration-contexts
3. 

