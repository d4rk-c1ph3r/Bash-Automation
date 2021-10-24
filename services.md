
# OpenSSH

```
sudo apt install opnessh-client
sudo apt install openssh-server
cat /etc/ssh/ssh_config   # client configuration
cat /etc/ssh/sshd_config  # server configuration
sudo systemctl restart sshd.service
sudo passwd -l root   # locking
sudo passwd -S root   # status
ssh-copy-id
```
