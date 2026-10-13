# Mission Reflection

Completing this laboratory helped me understand the importance of securing a server using a host-based firewall. A host-based firewall protects an individual server by controlling the network traffic entering and leaving it. Even if the physical network perimeter is breached, firewall rules can provide another layer of protection by restricting unauthorized connections.

Managing open network ports is also important because every accessible port may provide an entry point to a service. By allowing only the ports needed by the application, administrators can reduce the server's attack surface. In this activity, I learned how to allow SSH for remote administration and TCP port 8080 for the web application while applying a Default Deny incoming policy.

In a real enterprise environment, leaving a database port such as 3306 for MySQL open to the public internet can expose the database to unauthorized connection attempts and attacks. Attackers may try to exploit weak credentials or vulnerabilities in the database service. Database access should therefore be restricted to trusted systems and authorized users rather than being publicly accessible.

This mission changed my perspective on how easily a server can become exposed when security settings are overlooked. Before configuring UFW, I understood that servers needed protection, but this activity helped me see how firewall rules can control access to specific services. I also learned why SSH should be allowed before enabling the firewall on a remotely managed server.

With eight laboratory missions in my GitHub portfolio, I can see my progress in learning different areas of cloud computing. The activities have introduced me to infrastructure, deployment, data management, operations, and security. Each mission has helped me develop practical technical skills and improve my understanding of cloud environments.

Overall, this laboratory taught me that cloud security requires careful configuration, regular verification, and responsible management. I learned that even a simple firewall rule can make an important difference in protecting a server and its services.
