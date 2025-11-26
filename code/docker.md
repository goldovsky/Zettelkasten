# Docker

pour relancer docker si il y a un problème: 
```bash
sudo systemctl restart docker
```

### Others
```bash
#!/bin/bash

# -------------------------------
# Basic Docker Commands:
# -------------------------------
# List all containers (running and stopped)
docker ps -a

# List all running containers
docker ps

# Stop a running container
docker stop <container_id_or_name>

# Start a stopped container
docker start <container_id_or_name>

# Restart a container
docker restart <container_id_or_name>

# Remove a container
docker rm <container_id_or_name>

# Force-remove a running container
docker rm -f <container_id_or_name>

# Remove all stopped containers
docker container prune

# -------------------------------
# Managing Docker Images:
# -------------------------------
# List all Docker images
docker images

# Pull an image from Docker Hub
docker pull <image_name>

# Remove an image
docker rmi <image_id>

# Remove unused images
docker image prune

# Build an image from a Dockerfile in the current directory
docker build -t <image_name> .

# -------------------------------
# Working with Volumes:
# -------------------------------
# List all Docker volumes
docker volume ls

# Remove unused volumes
docker volume prune

# Remove a specific volume
docker volume rm <volume_name>

# -------------------------------
# Networks and Connectivity:
# -------------------------------
# List all Docker networks
docker network ls

# Inspect a specific network
docker network inspect <network_id_or_name>

# Create a new network
docker network create <network_name>

# Remove an unused network
docker network rm <network_name>

# Join a container to a network (while it’s running)
docker network connect <network_name> <container_id_or_name>

# Disconnect a container from a network
docker network disconnect <network_name> <container_id_or_name>

# -------------------------------
# Container Lifecycle:
# -------------------------------
# Run a container interactively
docker run -it <image_name>

# Run a container in detached mode
docker run -d <image_name>

# Run a container with a specific port mapping
docker run -p <host_port>:<container_port> <image_name>

# Run a container and bind-mount a directory
docker run -v $(pwd):/app <image_name>

# Inspect a container
docker inspect <container_id_or_name>

# View logs from a container
docker logs <container_id_or_name>

# Follow logs in real-time
docker logs -f <container_id_or_name>

# Execute a command inside a running container
docker exec -it <container_id_or_name> <command>
# Example:
# docker exec -it <container_id_or_name> bash

# -------------------------------
# Troubleshooting:
# -------------------------------
# Restart the Docker service
sudo systemctl restart docker

# Check Docker service status
sudo systemctl status docker

# Remove all unused resources (containers, networks, images)
docker system prune -a

# Inspect Docker logs
docker logs <container_id_or_name>

# Kill a container
docker kill <container_id_or_name>

# Display system-wide Docker information
docker info

# Show Docker disk-space usage
docker system df

# -------------------------------
# Other Useful Commands:
# -------------------------------
# Tag an image
docker tag <image_id> <repository>/<new_tag>

# Push an image to a repository
docker push <repository>/<image_name>

# Save an image as a tar archive
docker save -o <file_name>.tar <image_name>

# Load an image from a tar archive
docker load -i <file_name>.tar

# Copy files from a container to the host
docker cp <container_id>:<path_in_container> <path_on_host>

# Copy files from the host to a container
docker cp <path_on_host> <container_id>:<path_in_container>
```
