# Playing with Docker and HAProxy
Used this tutorial: https://medium.com/@nirgn/load-balancing-applications-with-haproxy-and-docker-d719b7c5b231

## To Run Locally
Build Dockerfile
`docker build -t awesome .`

Init Docker Swarm
`docker swarm init`

Deploy docker stack
`docker stack deploy --compose-file=docker-compose.yml prod`

Look at docker services
`docker service ls`

Update docker image for app
`docker service update --image awesome:v2 prod_awesome`
