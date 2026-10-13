# Laboratory 08: Cloud Security Engineer

## Mission Overview

This laboratory activity focuses on securing a Linux web server using the UFW firewall. It includes deploying an Nginx container, reviewing network access, and configuring rules to permit required services.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Configure a Default Deny incoming policy.
- Allow SSH and TCP port 8080.
- Document and verify firewall configurations.

## Commands Executed

```bash
docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl -I --max-time 5 http://localhost:8080
```

## Skills Learned

This laboratory helped me practice deploying a web server with Docker, testing an application using curl, configuring firewall rules, applying a Default Deny policy, and documenting network security settings.
