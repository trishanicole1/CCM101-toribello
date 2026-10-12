# Firewall Configuration

## Allow SSH Access

```bash
sudo ufw allow 22/tcp
This rule allows incoming SSH connections through port 22 so I can securely manage my server remotely.

Configure Default Deny Policy
bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
These rules block all incoming connections by default while allowing outgoing connections. This helps protect the server from unauthorized access.

Allow Port 8080
bash
sudo ufw allow 8080/tcp
This rule allows incoming TCP traffic on port 8080 for applications or web services that use this port.

What Would Happen If sudo ufw enable Ran Before sudo ufw allow ssh?
If I enabled the firewall before allowing SSH, I could lose my remote SSH connection if the firewall blocks incoming SSH traffic. This would make it difficult to access and manage the server remotely. To prevent this, I should allow SSH before enabling the firewall.

