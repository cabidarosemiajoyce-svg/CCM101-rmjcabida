# Mission 6 Reflection

## Reflection

Writing a `docker-compose.yml` file made the deployment process easier and more organized because the configuration for multiple containers could be placed in one file. Instead of manually typing many commands to configure the Nextcloud application and MariaDB database separately, Docker Compose allowed me to define both services together and deploy them using one command. This helped me understand how Infrastructure as Code can make cloud deployment more consistent and manageable.

I also learned that YAML indentation is very important. YAML uses spaces to identify the structure of the configuration. If I use incorrect indentation or a Tab instead of spaces, Docker Compose may not be able to read the file correctly, which can result in a configuration or deployment error. This taught me to carefully check the formatting of configuration files.

Environment variables were used to provide important configuration information to the containers. Variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` provide the database information required by the application. The `MYSQL_HOST` variable also tells the Nextcloud application which service provides the database.

Deploying Nextcloud was a useful experience because I was able to see how a cloud application could be deployed using containers and accessed through a browser. Seeing the Nextcloud setup page after running Docker Compose helped me connect the commands I entered in the terminal with an actual working application.

Since Mission 1, my understanding of Cloud Computing has developed from learning basic cloud concepts to understanding how containers, networking, configuration files, and automation can be used together. Mission 6 helped me understand that cloud deployment is not only about running commands but also about creating organized and repeatable infrastructure.
