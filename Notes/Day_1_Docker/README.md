# Day 1 - Docker Notes

Progress

✅ Lab 1: Run Your First Container
Concepts Covered
Introduction to containers
Running Docker containers
Managing container lifecycle
Container isolation
Linux namespaces
Control Groups (cgroups)
Docker Commands Practiced
docker container run
docker container ls
docker container ls -a
docker container exec
docker container stop
docker container prune
docker system prune
Key Learnings
Containers are lightweight isolated environments used to run applications.
Containers use Linux namespaces for isolation.
cgroups control and limit resource usage such as CPU and memory.
Multiple containers can run on the same host without dependency conflicts.
Containers include their required dependencies, reducing environment setup issues.
✅ Lab 2: Add CI/CD Value with Docker Images
Docker Images

Learned that Docker images are read-only templates used to create containers.

An image contains:

Application code
Dependencies
Libraries
Runtime environment
Configuration files
Creating a Custom Docker Image

Created a custom Docker image using a Dockerfile.

Project Structure
Docker-Learning-Journey/

├── Dockerfile
├── app.txt
└── README.md
Dockerfile Used
FROM ubuntu

COPY app.txt /app.txt

CMD ["cat", "/app.txt"]
Dockerfile Instructions Learned
FROM

Defines the base image.

Example:

FROM ubuntu
COPY

Copies files from the local machine into the image.

Example:

COPY app.txt /app.txt
CMD

Defines the command executed when the container starts.

Example:

CMD ["cat", "/app.txt"]
Building the Docker Image

Command:

docker build -t docker-lab2 .

This command:

Reads the Dockerfile
Creates image layers
Builds a custom Docker image
Running the Custom Image

Command:

docker run docker-lab2

Output:

Hello! This is my first custom Docker image.

Skills Learned
✅ Docker CLI
✅ Container management
✅ Docker images
✅ Dockerfile creation
✅ Custom image building
✅ Container isolation
✅ Linux namespaces
✅ cgroups
✅ Basic DevOps workflow
