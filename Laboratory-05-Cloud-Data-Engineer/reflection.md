# Mission Reflection

This laboratory activity helped me understand why different cloud storage models are designed for different purposes. For a photo-sharing application that needs to store millions of user-uploaded images, object storage is appropriate because images are unstructured data that can be stored as individual objects. Instead of treating the storage like a traditional hard drive, the application can organize objects inside buckets and access them through storage services and APIs.

Using Docker made the MinIO deployment easier because I did not have to manually install and configure every component of the storage server. I was able to create and start the MinIO container with one Docker command while configuring the required ports and administrator credentials. The `docker ps` command also provided a simple way to verify that the container was running.

A bucket is a logical container used to organize objects in an object storage system. In this activity, I created a bucket named `client-photos` and used it as the storage location for the sample file that I uploaded through the MinIO Web Console.

Large enterprise companies can reduce the risk of losing object storage data by using redundancy, replication, backups, versioning, and multiple storage locations. These methods provide additional copies or recovery options so that data can remain available even if a physical server or storage device fails.

My confidence in navigating the Linux command line is also growing because I was able to use Docker commands and understand their output. I practiced commands such as `docker pull`, `docker run`, and `docker ps`. I also learned that troubleshooting requires reading error messages carefully and adjusting commands based on the actual environment. Overall, this activity gave me more practical experience with Linux, Docker, and cloud storage and helped me understand how these tools work together in a cloud computing environment.
