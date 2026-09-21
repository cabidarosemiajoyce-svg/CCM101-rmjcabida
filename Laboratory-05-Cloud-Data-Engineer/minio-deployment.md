# MinIO Deployment Documentation

## Deployment Overview

For this laboratory activity, I deployed **MinIO**, an S3-compatible object storage server, inside the KillerCoda Ubuntu Playground using Docker.

The goal of the deployment was to create a working proof-of-concept object storage environment for the client's photo-sharing application. After starting the MinIO container, I accessed its Web Console, created the required bucket, and uploaded a sample file.

## 1. Docker Deployment

The MinIO container was started using the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
```

The MinIO image was obtained from the `quay.io/minio/minio` registry.

### Command Breakdown

| Option                               | Purpose                                                             |
| ------------------------------------ | ------------------------------------------------------------------- |
| `docker run`                         | Creates and starts a new Docker container.                          |
| `-d`                                 | Runs the container in detached mode.                                |
| `-p 9000:9000`                       | Maps the MinIO API port from the container to the host environment. |
| `-p 9001:9001`                       | Maps the MinIO Web Console port to the host environment.            |
| `--name minio-server`                | Assigns the container the name `minio-server`.                      |
| `-e`                                 | Sets an environment variable inside the container.                  |
| `MINIO_ROOT_USER=cloudadmin`         | Sets the MinIO administrator username.                              |
| `MINIO_ROOT_PASSWORD=CloudNova2026!` | Sets the MinIO administrator password.                              |
| `server /data`                       | Starts MinIO in server mode using `/data` as its storage location.  |
| `--console-address ":9001"`          | Configures the MinIO Web Console to use port `9001`.                |

Docker's `-e` or `--env` option is used to provide environment variables to a running container. These variables allowed the MinIO administrator credentials to be configured when the container was created.

## 2. Container Verification

After starting the container, I verified that MinIO was running with:

```bash
docker ps
```

The command showed the `minio-server` container with an active status and the required port mappings.

The deployment screenshot is stored at:

```text
screenshots/minio-deployed.png
```

## 3. Web Console Access

The MinIO Web Console was accessed using:

```text
Port: 9001
```

The port was opened through the KillerCoda port access feature.

The credentials configured during deployment were:

```text
Username: cloudadmin
Password: CloudNova2026!
```

Port `9000` was also mapped because it is used by the MinIO API, while port `9001` was used for the Web Console in this deployment.

## 4. Bucket Creation

After logging into the MinIO Web Console, I created the required bucket:

```text
client-photos
```

The bucket was used to organize the objects uploaded for the laboratory activity.

## 5. Object Upload

Inside the `client-photos` bucket, I uploaded a sample file to verify that the object storage service was functioning correctly.

The upload screenshot is stored at:

```text
screenshots/minio-bucket-upload.png
```

## 6. Deployment Result

The deployment was successfully verified through both the Docker command line and the MinIO Web Console. The running container confirmed that the MinIO service was active, while the successful bucket creation and file upload demonstrated that the object storage environment was operational.

## Technical Reference

* Docker documentation — `docker run` and environment variables
* MinIO documentation — MinIO object storage and server configuration
* AWS documentation — Object Storage and Amazon S3 concepts
