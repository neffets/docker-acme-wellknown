# docker-acme-wellknown
haproxy plugin for renewal of letsencrypt certificates

## swarm mode

> docker stack deploy -c docker-compose.yml wellknown

## why

add this to your docker swarm with haproxy (I recommend "dockercloud/haproxy":https://github.com/docker/dockercloud-haproxy )

set setting VIRTUAL_HOST_WEIGHT=99 for make the acme wellknown rule the top one.

see "letsencrypt project":https://letsencrypt.org/ too.

## docker

Get automated build image from:

> docker pull neffets/acme-wellknown

