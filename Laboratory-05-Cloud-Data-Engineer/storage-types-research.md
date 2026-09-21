# Storage Types Research

## Overview

Cloud storage provides different ways to store and access data depending on the requirements of an application. The three primary storage models are **Block Storage, File Storage, and Object Storage**. Each model is designed for different access patterns, performance requirements, and types of workloads.

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                                                                         | Primary Use Case                                                                                                 | Cloud Provider Example                        |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks. These blocks are presented to a system as a storage volume that can be formatted and used like a disk.            | Operating systems, virtual machine disks, databases, and applications requiring low-latency block-level access.  | **Amazon Elastic Block Store (Amazon EBS)**   |
| **File Storage**   | Stores data as files organized within directories and folders. It provides a shared file-system structure that can be accessed by multiple systems. | Shared documents, content repositories, application files, and workloads that require shared file-system access. | **Amazon Elastic File System (Amazon EFS)**   |
| **Object Storage** | Stores data as individual objects together with metadata and a unique identifier. Objects are organized inside storage containers called buckets.   | Large amounts of unstructured data such as images, videos, backups, archives, and application-generated content. | **Amazon Simple Storage Service (Amazon S3)** |

##  Why Object Storage is the best choice for storing their user-uploaded images. 

Object Storage is an appropriate choice for the client's photo-sharing application because user-uploaded images are unstructured data and may grow to millions of objects. It is designed for large-scale storage and provides an application-friendly way to store and retrieve objects through APIs. For this proof of concept, MinIO provides an S3-compatible object storage environment that demonstrates the same general object-storage model used by services such as Amazon S3.


