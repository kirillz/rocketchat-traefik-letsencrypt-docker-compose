# Rocket.Chat with Let's Encrypt in a Docker Compose

Install the Docker Engine by following the official guide: https://docs.docker.com/engine/install/

Install the Docker Compose by following the official guide: https://docs.docker.com/compose/install/

Deploy Rocket.Chat server with a Docker Compose using the command:

`docker-compose -f rocketchat-traefik-letsencrypt-docker-compose.yml -p rocketchat up -d`

!!! Остановка всех контейнеров
`docker stop $(docker ps -a -q)`
!!! Удаление всех контейнеров
`docker rmi -f $(docker images -q)`
