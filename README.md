# Docker Commands

Welcome to the **Docker Commands** repository! This repository contains a list of useful Docker commands that help streamline working with Docker images and containers. Whether you're managing containers or building images, these commands will assist you in your daily tasks.

## Table of Contents

1. [Working with Images](#working-with-images)
2. [Working with Containers](#working-with-containers)
3. [Helpful Commands](#helpful-commands)
4. [Resources](#resources)

---

## Working with Images

Docker images are the foundation of containers. Below are some useful commands to manage and manipulate Docker images.

- **List Docker Images**
  ```bash
  docker images
  ```
  or
  ```bash
  docker image ls
  ```
  Displays a list of all the Docker images available on your system.

- **Remove Docker Image(s)**
  ```bash
  docker rmi <image> [image...]
  ```
  or
  ```bash
  docker image rm <image> [image...]
  ```
  Removes the specified image(s) from your local repository.

---

## Working with Containers

Docker containers are lightweight, portable, and self-sufficient units that contain everything necessary to run your application. Here are some essential commands to manage them:

- **Run a Container from an Image**
  ```bash
  docker run <image>
  ```
  Launches a container based on the specified image.

  - **Assign a Name to the Container**
    ```bash
    docker run --name <name> <image>
    ```
    Starts a container with a specific name.

  - **Automatically Remove the Container After It Exits**
    ```bash
    docker run --rm <image>
    ```
    Deletes the container once it stops running.

  - **Start a Container in Interactive Mode**
    ```bash
    docker run -it <image>
    ```
    Opens an interactive session with the container.

  - **Run a Container in Detached Mode**
    ```bash
    docker run -d <image>
    ```
    Runs the container in the background.

- **List Running Containers**
  ```bash
  docker ps
  ```
  Shows a list of all currently running containers.

  - **List All Containers**
    ```bash
    docker ps -a
    ```
    Shows both running and stopped containers.

- **Stop a Running Container**
  ```bash
  docker stop <container> [container...]
  ```
  Stops one or more containers.

- **Start a Stopped Container**
  ```bash
  docker start <container> [container...]
  ```
  Restarts one or more stopped containers.

- **Remove a Container**
  ```bash
  docker rm <container> [container...]
  ```
  Deletes one or more containers.

- **Execute a Command in a Running Container**
  ```bash
  docker exec <container> <command>
  ```
  Runs a command inside a running container.

  - **Execute Bash in a Running Container**
    ```bash
    docker exec -it <container> bash
    ```
    Starts an interactive bash session inside the container.

---

## Helpful Commands

In addition to managing images and containers, Docker provides several other commands to make your work more efficient:

- **View Container Logs**
  ```bash
  docker logs <container>
  ```
  Shows logs from a running or stopped container.

- **Monitor Resource Usage**
  ```bash
  docker stats
  ```
  Displays real-time stats (CPU, memory, network, etc.) for running containers.

- **Remove All Stopped Containers**
  ```bash
  docker container prune
  ```
  Deletes all stopped containers.

- **Clean Up Unused Docker Objects**
  ```bash
  docker system prune
  ```
  Removes all unused containers, networks, images (not referenced by any container), and optionally, volumes.

---

## Resources

For more detailed information on Docker and its usage, check out the official Docker documentation:

- [Docker Documentation](https://docs.docker.com)
- [Docker Command Line Reference](https://docs.docker.com/engine/reference/commandline/docker/)

Feel free to contribute additional commands or tips by submitting a pull request. Happy Dockering!

---
