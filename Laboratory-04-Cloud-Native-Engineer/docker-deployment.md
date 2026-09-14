# Docker Deployment

## Checkpoint 3 - Docker Verification

### Docker Version

```bash
docker --version
```

I used this command to check if Docker was installed and to see the Docker version available in the KillerCoda environment.

### Docker Information

```bash
docker info
```

I used this command to check the current Docker environment and make sure the Docker service was working.

## Checkpoint 4 - Nginx Deployment

### Pull Nginx

```bash
docker pull nginx
```

This command downloaded the Nginx image that I needed for the web server.

### Run Nginx

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command created and started the Nginx container in the background and connected port 8080 of the host to port 80 of the container.

### Test Nginx

```bash
curl http://localhost:8080
```

I used this command to check if the Nginx web server was running, and it returned the Nginx welcome page HTML.

## Checkpoint 5 - Container Lifecycle

### List Running Containers

```bash
docker ps
```

This command showed me the Nginx container while it was running.

### Stop the Container

```bash
docker stop nginx-server
```

This command stopped the running Nginx container.

### Verify the Container Is Stopped

```bash
docker ps
```

The Nginx container was no longer displayed because it was already stopped.

### Remove the Container

```bash
docker rm nginx-server
```

This command completely removed the stopped Nginx container.

### Verify the Removal

```bash
docker ps -a
```

I used this command to check all containers and verify that the Nginx container was removed.
