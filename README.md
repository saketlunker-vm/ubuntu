# ubuntu

# Update
```
sudo apt-get update
```
Use apt over https repository
```
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
```
Add docker GCP Key
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
Install Docker
```
sudo apt-get install docker-ce docker-ce-cli containerd.io
```

