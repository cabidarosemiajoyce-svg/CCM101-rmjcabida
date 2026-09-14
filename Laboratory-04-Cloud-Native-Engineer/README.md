# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I learned about the difference between Virtual Machines and containers. I also used KillerCoda to practice Docker commands and deployed an Nginx web server inside a container. The activity helped me understand how containerization can make application deployment faster and more lightweight.

## Objectives

* Understand the difference between Virtual Machines and containers.
* Use a Docker-enabled Linux environment.
* Practice basic Docker commands.
* Pull and run an Nginx container.
* Test a web server using curl.
* Manage the lifecycle of a Docker container.
* Document my work using Markdown and GitHub.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
docker ps -a
```

## Skills Learned

I learned how to check a Docker environment, download a Docker image, create and run a container, connect ports, and manage a container. I also learned how to use curl to test a web server and how to organize my laboratory files and screenshots in GitHub.

## Challenges Encountered

One challenge I experienced was understanding the port mapping in the Docker run command. At first, I needed to understand why port 8080 was used on the host while Nginx was using port 80 inside the container. After running the command and testing it with curl, I understood how the two ports were connected.
