# ubuntu

## Installing Docker

### Updating
```
sudo apt-get update
```
### Installing Components to use apt over https repository
```
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
```
### Adding Docker GPG Key
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
### Selecting stable build for our Ubuntu Distro
```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
### Installing Docker
```
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
```
### Display Docker version
```
docker -v
```
## Creating Ubuntun Container
### Pulling Ubuntu Image
```
sudo docker pull ubuntu:latest
```
### Creating a Interactive Ubuntu Container
```
sudo docker run -it --name ubuntu1 --hostname ubuntu1 ubuntu:latest /bin/bash
```
#### Display Ubuntu Version in Container
```
apt update
apt lsb-release
lsb_release -a
```
#### Exit the container
```
exit
```
