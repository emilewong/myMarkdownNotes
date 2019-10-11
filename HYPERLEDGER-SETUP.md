# Hyperledger Environment on Ubuntu

## Prerequisites
Before we begin, if you haven’t already done so, you may wish to check that you have all the prerequisites below installed on the platform(s) on which you’ll be developing blockchain applications and/or operating Hyperledger Fabric.

  - Install cURL
  - Install Git
  - Docker and Docker Compose
  - Go Programming Language
  - Node.js Runtime and NPM
  - Python


### Update ubuntu
```sh
sudo apt update
sudo apt -y upgrade
sudo reboot now
```
### Install cURL

```sh
$ sudo apt install curl
```
Test curl
```sh
curl http://google.com
curl --version
```
### Install Git
```sh
sudo apt install git
```
Check git
```sh
git --version
```
### Python
```sh
sudo apt install -y python-minimal
```
Check Python
```sh
python --version
```
### Install required packages
```sh
sudo apt install apt-transport-https ca-certificates gnupg-agent software-properties-common
```
### Install Docker
Download Docker
```sh
curl-fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
Add repository
```sh
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```
Install docker ce
```sh
sudo apt -y install docker-ce
```
Change Mod
```sh
sudo usermod -aG docker [your username]
```
Check docker
```sh
docker -v
```
or 
```sh
docker --version
```
Download docker-compose
```sh
sudo curl -L https://github.com/docker/compose/releases/download/1.18.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
```
Change access right
```sh
sudo chmod +x /usr/local/bin/docker-compose
```
Restart computer
```sh
sudo reboot now
```

Update the system again
```sh
sudo apt update
sudo apt -y upgrade

```

Download Go programming language
```sh
wget https://dl.google.com/go/go1.12.7.linux-amd64.tar.gz
```
Extract the package
```sh
sudo tar -xvf go1.12.7.linux-amd64.tar.gz
```
Move the package to user local
```sh
sudo mv go /usr/local
```




