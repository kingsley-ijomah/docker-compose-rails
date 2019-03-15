# README

This is a sample project that spins up 3 services in different containers that could talk to each other

Gettings this up and running

# build our images
------------------
docker-compose build --force-rm

# spin up all containers
------------------------
docker-compose up -d

# setup database within our container
-------------------------------------
docker-compose run --rm app rails db:create db:migrate

# example of running console
----------------------------
docker-compose run --rm app rails console