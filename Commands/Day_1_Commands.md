# Docker Basic Commands

## Check Docker Version

```bash
docker --version
```

Displays the installed Docker version.

---

## View Docker Information

```bash
docker info
```

Displays detailed Docker system information.

---

## Run the Hello World Container

```bash
docker run hello-world
```

Downloads (if needed) and runs the Hello World container.

---

## List Running Containers

```bash
docker ps
```

Shows only currently running containers.

---

## List All Containers

```bash
docker ps -a
```

Shows both running and stopped containers.

---

## Start a Stopped Container

```bash
docker start <container_id>
```

Example:

```bash
docker start a1b2c3d4
```

---

## Stop a Running Container

```bash
docker stop <container_id>
```

---

## Restart a Container

```bash
docker restart <container_id>
```

---

## Remove a Container

```bash
docker rm <container_id>
```

Container must be stopped before removing.

---

## Remove a Running Container Forcefully

```bash
docker rm -f <container_id>
```

---

## List Docker Images

```bash
docker images
```

Displays all downloaded images.

---

## Download an Image

```bash
docker pull ubuntu
```

Downloads the Ubuntu image.

---

## Run an Ubuntu Container

```bash
docker run ubuntu
```

---

## Run Interactive Ubuntu Container

```bash
docker run -it ubuntu
```

Starts Ubuntu with an interactive terminal.

---

## Exit a Container

```bash
exit
```

Leaves the container.

---

## Run Container in Detached Mode

```bash
docker run -d nginx
```

Runs the container in the background.

---

## View Container Logs

```bash
docker logs <container_id>
```

---

## Execute Command Inside Running Container

```bash
docker exec -it <container_id> bash
```

Example:

```bash
docker exec -it 7e2f4 bash
```

---

## Show Docker Images

```bash
docker image ls
```

---

## Remove an Image

```bash
docker rmi <image_id>
```

---

## Build an Image from Dockerfile

```bash
docker build -t myimage .
```

Builds a Docker image using the Dockerfile in the current directory.

---

## List Images After Build

```bash
docker images
```

Shows the newly created image.

---

## Run Your Custom Image

```bash
docker run myimage
```

---

## Tag an Image

```bash
docker tag myimage myimage:v1
```

Creates a tagged version of the image.

---

## Remove Dangling Images

```bash
docker image prune
```

Deletes unused dangling images.
