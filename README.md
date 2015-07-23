##Useful Docker Commands##

- List all docker images

<code>
docker images
</code>

- List all running docker containers

<code>
docker ps
</code>

- Run a specific docker image

<code>
docker run <i>image id</i>
</code>

- Remove a specific docker image

<code>
docker rmi <i>image id</i>
</code>

- Run an image in the background

<code>
docker run <i>image id</i> -d
</code>

- Stop a docker container

<code>
docker stop <i>container id</i>
</code>

- Force remove all docker images 

<code>
docker rmi -f $(docker images -q)
</code>

- Force stop all docker containers

<code>
docker stop $(docker ps -a -q)
</code>

- Force remove all docker containers which have an exited status

<code>
docker rm $(docker ps --all -q -f status=exited)
</code>

- Execute a bash command inside a running container

<code>
docker exec -it <i>container id</i> sh -c <i>bash command</i>
</code>

## Docker Machine Commands ##

- List all docker machines

<code>
docker-machine ls
</code>

- Remove a docker machine by name

<code>
docker-machine rm <i>machine name</i>
</code>

## Docker Compose Commands ##

- Build and run a multi container app

<code>
docker-compose up
</code>