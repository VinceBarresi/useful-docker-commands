## Useful Docker Commands

- List all docker images

<code>
<t>docker images</t>
</code>

- List all running docker containers

<code>
<t>docker ps</t>
</code>

- List all docker containers

<code>
<t>docker ps -a</t>
</code>

- Run a specific docker image

<code>
<t>docker run <i>image id</i></t>
</code>

- Remove a specific docker image

<code>
<t>docker rmi <i>image id</i></t>
</code>

- Run an image in the background

<code>
<t>docker run <i>image id</i> -d</t>
</code>

- Stop a docker container

<code>
<t>docker stop <i>container id</i></t>
</code>

- Force remove all docker images 

<code>
<t>docker rmi -f $(docker images -q)</t>
</code>

- Force stop all docker containers

<code>
<t>docker stop $(docker ps -a -q)</t>
</code>

- Force remove all docker containers which have an exited status

<code>
<t>docker rm $(docker ps --all -q -f status=exited)</t>
</code>

- Execute a bash command inside a running container

<code>
<t>docker exec -it <i>container id</i> sh -c <i>bash command</i></t>
</code>

- SSH into container to run bash commands

<code>
<t>docker exec -it <i>container id</i> bash</t>
</code>

## Docker Machine Commands ##

- List all docker machines

<code>
<t>docker-machine ls</t>
</code>

- Remove a docker machine by name

<code>
<t>docker-machine rm <i>machine name</i></t>
</code>

## Docker Compose Commands ##

- Build and run a multi container app

<code>
<t>docker-compose up</t>
</code>
