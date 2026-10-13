
# Firewall Configuration

## Command to Allow SSH

```bash
sudo ufw allow ssh
```

## Commands to Set the Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Command to Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

## What Happens If UFW Is Enabled Before Allowing SSH?

If I run `sudo ufw enable` before `sudo ufw allow ssh`, incoming SSH connections may be blocked by the default deny policy, potentially disconnecting me from the remote server.

