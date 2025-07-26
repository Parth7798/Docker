# 🐳 Docker Cheat Sheet

A comprehensive, quick-reference guide covering essential Docker commands categorized for ease of use. Perfect for beginners and professionals managing containers, images, networks, and services in Docker environments.

---

## 📚 Index

1. [Docker Build Commands](#1-docker-build-commands)  
2. [Docker Clean Up Commands](#2-docker-clean-up-commands)  
3. [Container Interaction Commands](#3-container-interaction-commands)  
4. [Image Commands](#4-image-commands)  
5. [Container Inspection Commands](#5-container-inspection-commands)  
6. [Docker Run Commands](#6-docker-run-commands)  
7. [Docker Registry Commands](#7-docker-registry-commands)  
8. [Docker Network Commands](#8-docker-network-commands)  
9. [Docker Service Commands](#9-docker-service-commands)  
10. [Docker Volume Commands](#10-docker-volume-commands)  
11. [Docker Swarm Commands](#11-docker-swarm-commands)  
12. [Docker Filesystem Commands](#12-docker-filesystem-commands)  
13. [Docker Environment Variables](#13-docker-environment-variables)  
14. [Docker Health Checks](#14-docker-health-checks)  
15. [Docker Compose Commands](#15-docker-compose-commands)  
16. [Docker Stats](#16-docker-stats)  

---

## 1. Docker Build Commands

| Command | Description |
|--------|-------------|
| `docker build -t <image_name> .` | Build image from Dockerfile in current directory |
| `docker build --no-cache -t <image_name> .` | Build image without cache |
| `docker build -f <dockerfile_name> -t <image_name> .` | Build using specified Dockerfile |

---

## 2. Docker Clean Up Commands

| Command | Description |
|--------|-------------|
| `docker system prune` | Remove all unused data |
| `docker container prune` | Remove stopped containers |
| `docker image prune` | Remove unused images |
| `docker volume prune` | Remove unused volumes |
| `docker network prune` | Remove unused networks |

---

## 3. Container Interaction Commands

| Command | Description |
|--------|-------------|
| `docker run <image_name>` | Run a container |
| `docker start <container_id>` | Start a container |
| `docker stop <container_id>` | Stop a container |
| `docker restart <container_id>` | Restart a container |
| `docker exec -it <container_id> <command>` | Run command in running container |

---

## 4. Image Commands

| Command | Description |
|--------|-------------|
| `docker images` | List images |
| `docker pull <image_name>` | Download image |
| `docker push <image_name>` | Upload image |
| `docker rmi <image_id>` | Remove image |

---

## 5. Container Inspection Commands

| Command | Description |
|--------|-------------|
| `docker ps` | List running containers |
| `docker ps -a` | List all containers |
| `docker logs <container_id>` | View container logs |
| `docker inspect <container_id>` | View detailed container info |

---

## 6. Docker Run Commands

| Command | Description |
|--------|-------------|
| `docker run -d <image_name>` | Run in detached mode |
| `docker run -p <host_port>:<container_port> <image_name>` | Map ports |
| `docker run -v <host_path>:<container_path> <image_name>` | Mount volume |
| `docker run --name <container_name> <image_name>` | Name the container |

---

## 7. Docker Registry Commands

| Command | Description |
|--------|-------------|
| `docker login` | Log into registry |
| `docker logout` | Log out of registry |
| `docker search <term>` | Search registry |
| `docker pull <registry>/<image_name>` | Pull from registry |

---

## 8. Docker Network Commands

| Command | Description |
|--------|-------------|
| `docker network create <name>` | Create network |
| `docker network ls` | List networks |
| `docker network inspect <name>` | Inspect network |
| `docker network connect <network> <container>` | Connect container to network |

---

## 9. Docker Service Commands

| Command | Description |
|--------|-------------|
| `docker service create --name <name> <image>` | Create a service |
| `docker service ls` | List services |
| `docker service scale <name>=<replicas>` | Scale service |
| `docker service logs <name>` | View service logs |

---

## 10. Docker Volume Commands

| Command | Description |
|--------|-------------|
| `docker volume create <name>` | Create volume |
| `docker volume ls` | List volumes |
| `docker volume inspect <name>` | Inspect volume |
| `docker volume rm <name>` | Remove volume |

---

## 11. Docker Swarm Commands

| Command | Description |
|--------|-------------|
| `docker swarm init` | Init Swarm |
| `docker swarm join` | Join Swarm |
| `docker node ls` | List Swarm nodes |
| `docker service create` | Create Swarm service |
| `docker service scale` | Scale Swarm service |

---

## 12. Docker Filesystem Commands

| Command | Description |
|--------|-------------|
| `docker cp <container>:<path> <host>` | Copy from container |
| `docker cp <host
