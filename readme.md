# Vagrant

Build docker environment in vagrant

## start vm
```
start.bat
```

## initial
```
vagrant ssh

# upgrade package
sudo apt-get update && sudo apt-get -y upgrade

exit

vagrant.exe provision
```

## use key to login host

### Open Powershell
```
run powershell as administrator
```
### Create ssh key for login
```
ssh-keygen.exe -t rsa -b 2048 -C "vagrant"
```
### copy pub key to target
```
scp ~/.ssh/id_rsa.pub vagrant@x.x.x.x:.
```
### Use password to log in to the host
```
ssh vagrant@x.x.x.x
```
### add public key to authorized_keys
```
cat id_rsa.pub >> .ssh/authorized_keys
```

