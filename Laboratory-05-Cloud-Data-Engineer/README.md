# Laboratory 05 – The Cloud Data Engineer

## Mission Overview

This laboratory activity focuses on cloud storage and object storage technologies. The activity begins by comparing **Block Storage, File Storage, and Object Storage** and identifying the types of workloads suited to each storage model.

For the practical portion of the mission, I deployed **MinIO**, an S3-compatible object storage server, using Docker in the KillerCoda Ubuntu Playground. I configured the server using environment variables, mapped the required ports, accessed the MinIO Web Console, created a bucket named `client-photos`, and uploaded a sample object.

The activity demonstrates a basic cloud storage workflow and shows how object storage can be used to store large amounts of unstructured data separately from an application server.

---

## Objectives

The objectives of this laboratory activity were to:

- Differentiate between Block, File, and Object Storage.
- Identify appropriate use cases for different cloud storage models.
- Deploy an S3-compatible object storage server using Docker.
- Configure a container using environment variables.
- Map and access a cloud service through specific ports.
- Access the MinIO Web Console through port `9001`.
- Create an object storage bucket.
- Upload and verify an object inside the bucket.
- Document technical procedures using Markdown.
- Maintain and expand a professional GitHub Cloud Computing portfolio.

---

## Tools Used

| Tool | Purpose |
|---|---|
| **KillerCoda** | Provided the browser-based Ubuntu/Docker laboratory environment. |
| **Ubuntu Linux** | Provided the command-line environment for the deployment. |
| **Docker** | Used to deploy MinIO as a containerized service. |
| **MinIO** | Provided the S3-compatible object storage service. |
| **Web Browser** | Used to access the MinIO Web Console. |
| **GitHub** | Used to document and store the laboratory portfolio. |
| **Markdown** | Used to create the required documentation files. |

---

## Skills Learned
```
Through this laboratory activity, I learned how Block Storage, File Storage, and Object Storage differ in the way they organize and provide access to data. I also learned that choosing the appropriate storage type depends on the requirements and workload of an application. I practiced using Docker to deploy a containerized service and learned how to use Docker options for port mapping, environment variables, container naming, and detached execution. I also learned how to access the MinIO Web Console, create a bucket, and upload an object, which helped me understand the basic workflow of an S3-compatible object storage service. In addition, I gained more experience using the Linux command line through Docker commands such as `docker pull`, `docker run`, and `docker ps`. Finally, I practiced organizing technical information using Markdown and maintaining screenshots as evidence inside a GitHub repository.
```
---

