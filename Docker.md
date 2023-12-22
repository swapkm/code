### System Start-Stop
`sudo systemctl start docker`

`sudo systemctl stop docker`

`sudo systemctl stop docker.socket`

`sudo systemctl restart docker`

`sudo systemctl status docker`

`sudo systemctl enable docker`

`sudo systemctl disable docker`

### Start-Stop Docker
`sudo service docker start`

`sudo service docker stop`

### Pull Image From DockerHub
`sudo docker pull wordpress`

### See All Docker Imagees
`sudo docker images`

### Remove Docker Images
`sudo docker rmi 45458imageid57459`

`sudo docker rmi imagename`

### Remove all images at onece
`sudo docker image prune`

-----------------------------------------------------
### List All Curent Running Docker Container
`sudo docker ps`

`sudo docker ps -a`

### Start Docker Container Using Name or ID
`sudo docker start nameofcontainer`

`sudo docker start 8473895containerid795`

### Stop Container
`sudo docker stop 75498conarinerid8547`

`sudo docker stop nameofcontainer`

### Remove Docker Container
`sudo docker rm 12364485containerid987459`

`sudo docker rm name`

### Remove all at once
`sudo docker container prune`
