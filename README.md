#  Docker Cheat Sheet

# INDEX

1.​ Docker Build Commands 

2.​ Docker Clean Up Commands

3.​ Container Interaction Commands

4.​ Image Commands 

5.​ Container Inspection Commands 

6.​ Docker Run Commands 

7.​ Docker Registry Commands 

8.​ Docker Network Commands 

9.​ Docker Service Commands 

10.​Docker Volume Commands 

11.​Docker Swarm Commands 

12.​Docker Filesystem Commands 

13.​Docker Environment Variables 

14.​Docker Health Checks

15.​Docker Compose Commands 

16.​Docker Stats 





1.​ Docker Build Commands:


| Commands  | Description  |
| --- | --- |
| docker build -t &lt;image_name&gt; .  | Build a Docker image using the Dockerfile in the current directory.  |
| docker build --no-cache -t <br>&lt;image_name&gt; .  | Build a Docker image without using the <br>cache.  |
| docker build -f &lt;dockerfile_name&gt; -t <br>&lt;image_name&gt; .  | Build a Docker image using a specified <br>Dockerfile.  |


2.​ Docker Clean Up Commands:


| Commands  | Description  |
| --- | --- |
| docker system prune  | Remove all unused Docker resources, <br>including containers, images, networks, <br>and volumes.  |
| R docker container prune  | Remove all stopped containers.  |
| docker image prune  | Remove unused images.  |
| docker volume prune  | Remove unused volumes.  |
| A docker network prune  | Remove unused networks.  |


3.​ Container Interaction Commands:


| Commands  | Description  |
| --- | --- |
| docker run &lt;image_name&gt;  | Run a Docker image as a container.  |
| docker start &lt;container_id&gt;  | Start a stopped container.  |
| docker stop &lt;container_id&gt;  | Stop a running container.  |
| docker restart &lt;container_id&gt;  | Restart a running container.  |
| docker exec -it &lt;container_id&gt; <br>&lt;command&gt;  | Execute a command inside a running <br>container interactively.  |



4.​ Image Commands: 


| Commands  | Description  |
| --- | --- |
| docker images  | List available Docker images.  |
| docker pull &lt;image_name&gt;  | Pull a Docker image from a Docker <br>registry.  |
| docker push &lt;image_name&gt;  | Push a Docker image to a Docker <br>registry.  |
| docker rmi &lt;image_id&gt;  | Remove a Docker image.  |


5.​ Container Inspection Commands:


| Commands  | Description  |
| --- | --- |
| docker ps  | List running containers.  |
| docker ps -a  | List all containers, including stopped <br>ones.  |
| R docker logs &lt;container_id&gt;  | Fetch the logs of a specific container.  |
| docker inspect &lt;container_id&gt;  | Inspect detailed information about a <br>container.  |


6.​ Docker Run Commands:


| PCommands  | Description  |
| --- | --- |
| docker run -d &lt;image_name&gt;  | Run a Docker image as a container in <br>detached mode.  |
| docker run -p &lt;host_port&gt;:&lt;container_port&gt; &lt;image_name&gt;  | Publish container ports to the host.  |
| docker run -v <br>&lt;host_path&gt;:&lt;container_path&gt; <br>&lt;image_name&gt;  | Mount a host directory or volume to a <br>container.  |
| docker run --name &lt;container_name&gt; <br>&lt;image_name&gt;  | Assign a custom name to the container.  |


7.​ Docker Registry Commands: 


| Commands  | Description  |
| --- | --- |
| docker login  | Log in to a Docker registry.  |
| docker logout  | Log out from a Docker registry.  |
| docker search &lt;term&gt;  | Search for Docker images in a Docker <br>registry.  |
| docker pull &lt;registry&gt;/&lt;image_name&gt;  | Pull a Docker image from a specific <br>registry.  |


8.​ Docker Network Commands:


| Commands  | Description  |
| --- | --- |
| docker network create &lt;network_name&gt;  | Create a Docker network.  |
| R docker network ls  | List available Docker networks.  |
| docker network inspect &lt;network_name&gt;  | Inspect detailed information about a <br>Docker network.  |
| d&lt;ococknetar inneertw_Anoarkm ceo&gt;n nect &lt;network_name&gt;  | Connect a container to a Docker network.  |


9.​ Docker Service Commands:


| Commands  | Description  |
| --- | --- |
| docker service create --name <br>&lt;service_name&gt; &lt;image_name&gt;  | Create a Docker service from an image.  |
| docker service ls  | List running Docker services.  |
| docker service scale <br>&lt;service_name&gt;=&lt;replicas&gt;  | Scale the replicas of a Docker service.  |
| docker service logs &lt;service_name&gt;  | View logs of a Docker service.  |



10.​ Docker Volume Commands:


| Commands  | Description  |
| --- | --- |
| docker volume create &lt;volume_name&gt;  | Create a Docker volume.  |
| docker volume ls  | List available Docker volumes.  |
| docker volume inspect &lt;volume_name&gt;  | Inspect detailed information about a <br>Docker volume.  |
| docker volume rm &lt;volume_name&gt;  | H Remove a Docker volume.  |


11.​Docker Swarm Commands:


| Commands  | Description  |
| --- | --- |
| docker swarm init  | Initialize a Docker swarm on the current <br>node.  |
| R docker swarm join  | Join a Docker swarm as a worker node.  |
| docker node ls  | List the nodes in a Docker swarm.  |
| docker service create  | Create a service in the Docker swarm.  |
| A docker service scale  | Scale the replicas of a service in the <br>Docker swarm.  |


P12.​Docker Filesystem Commands:


| Commands  | Description  |
| --- | --- |
| docker cp <br>&lt;container_id&gt;:&lt;container_path&gt; <br>&lt;host_path&gt;  | Copy files from a container to the host.  |
| docker cp &lt;host_path&gt; <br>&lt;container_id&gt;:&lt;container_path&gt;  | Copy files from the host to a container.  |



13.​Docker Environment Variables:


| Commands  | Description  |
| --- | --- |
| -e or --env  | Set environment variables when running <br>a container.  |
| docker run -e &lt;variable_name&gt;=&lt;value&gt; &lt;image_name&gt;  | Set an environment variable when <br>running a container.  |


14.​Docker Health Checks:


| Commands  | Description  |
| --- | --- |
| HEALTHCHECK instruction  | TDefine a command to check the health of <br>a container.  |
| docker container inspect --format='{{json .State.Health}}' &lt;container_name&gt;  | Check the health status of a container.  |


15.​Docker Compose Commands:


| Commands  | Description  |
| --- | --- |
| A docker-compose up  | Create and start containers defined in a <br>Docker Compose file.  |
| P docker-compose down  | Stop and remove containers defined in a Docker Compose file.  |
| docker-compose ps  | List containers defined in a Docker <br>Compose file.  |
| docker-compose logs  | View logs of containers defined in a <br>Docker Compose file.  |


**16. Docker Stats:**


| Commands  | Description  |
| --- | --- |
| docker stats  | Display a live stream of resource usage<br>by containers.  |
| docker stats &lt;container_name&gt; | Display the resource usage of a specific<br>container.  |






