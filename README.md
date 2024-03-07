# ssh-setup
To set up an account with SSH

## Account details

```
sudo adduser --disabled-password --comment "" clint
sudo adduser clint sudo
sudo mkdir -p /home/clint/.ssh
echo "ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIMcr3liMpNWTijoMiVuE3Crrp+uDd3nLl20Hvjg7fC+D" > /home/clint/.ssh/authorized_keys
sudo chown clint:clint /home/clint/.ssh/authorized_keys

# In case there are issues with permissions
sudo chmod 700 /home/clint/.ssh/authorized_keys
sudo chmod 600 /home/clint/.ssh
```
