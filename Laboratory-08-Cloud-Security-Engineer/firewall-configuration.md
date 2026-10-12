# Firewall Configuration

## Allow SSH

```bash
sudo ufw allow ssh
```

## Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

## What would happen if `sudo ufw enable` ran before `sudo ufw allow ssh`?

If I enabled UFW before allowing SSH, incoming SSH connections could be blocked by the firewall's default deny policy. This could prevent me from accessing the server remotely and potentially lock me out. To avoid this, I should allow SSH first using `sudo ufw allow ssh` before enabling the firewall.
