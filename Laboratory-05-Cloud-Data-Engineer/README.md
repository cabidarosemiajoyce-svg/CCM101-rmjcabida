# Laboratory 05 – Cloud Data Engineer

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

Through this laboratory activity, I developed a better understanding of the three major cloud storage models: Block Storage, File Storage, and Object Storage, including how they organize data and support different application requirements. I also gained practical experience deploying a containerized service using Docker and learned how port mapping, environment variables, container naming, and detached execution are used when configuring a container. In addition, I learned how to manage an S3-compatible object storage service through the MinIO Web Console by creating a bucket and uploading an object. This activity also improved my confidence in using the Linux command line through Docker commands such as `docker pull`, `docker run`, and `docker ps`. Finally, I strengthened my technical documentation skills by organizing laboratory information in Markdown, maintaining screenshots as deployment evidence, and keeping the project properly structured in GitHub.

---

