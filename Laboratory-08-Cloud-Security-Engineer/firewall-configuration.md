# Firewall Configuration

## Allow SSH

Command used:

```bash
sudo ufw allow ssh
```

This command allows SSH connections so administrators can remotely manage the server.

## Configure the Default Deny Policy

Commands used:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming connections by default unless a firewall rule allows them. The second command allows outgoing connections by default.

## Allow Port 8080

Command used:

```bash
sudo ufw allow 8080/tcp
```

This command allows incoming TCP traffic through port 8080 for the web application.

## SSH Security Warning

If `sudo ufw enable` is executed before `sudo ufw allow ssh`, the firewall may block remote SSH access and lock out the administrator because incoming traffic is denied by default.
