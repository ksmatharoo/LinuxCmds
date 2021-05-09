# LinuxCmds

# check port is used by which process 
sudo lsof -i -P -n | grep 2181

# check file is used by which process
sudo lsof /var/lib/dpkg/lock-frontend

