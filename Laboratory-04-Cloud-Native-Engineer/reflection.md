# Mission Reflection

This laboratory helped me understand the difference between using a Virtual Machine and using a Docker container. When using a Virtual Machine, a complete operating system needs to be installed and started, so the setup can take more time and use more resources. In Docker, the Nginx container was created and started much faster because it uses the host operating system kernel instead of having its own complete operating system. From my experience in KillerCoda, I found the Docker setup easier and faster for this type of web server.

The port mapping `-p 8080:80` was important because it connected the host port 8080 to port 80 inside the Nginx container. The Nginx web server was running inside the container, so the mapping allowed me to access it through `http://localhost:8080`. When I used the curl command, I was able to see the Nginx welcome page, which showed that the connection was working.

When I used `docker rm`, the Nginx container was removed from Docker. The container itself and data stored only in its writable container layer are not kept as that container after it is removed. This is why important data should be stored using persistent storage such as Docker volumes when it needs to remain after a container is deleted.

Containerization can also improve teamwork between developers and IT operations teams. Developers can package an application with the environment it needs, while the operations team can run the same container in different environments. This supports the DevOps idea of making development and deployment more consistent.

My GitHub portfolio is also becoming more organized as I complete each laboratory activity. Laboratory 4 added Docker, containerization, technical documentation, and screenshots to my previous cloud computing work. It shows my progress and gives me a place where I can keep the skills and activities I learned throughout the course.
