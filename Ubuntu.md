# Ubuntu
Install filename.run
`chmod +x filenam*.run`
`sudo ./filenam*.run`
`unzip file.zip`
`unzip file.zip -d myfolder`

### If want to rename directory
`mv oldfolder newfolder`
`sudo dpkg -i filemane-*.deb`

## Docker

----------------------------------------------------
### Start-Stop Docker
`sudo service docker start`
`sudo service docker stop`

### Pull Image From DockerHub
`sudo docker pull wordpress`

### See All Docker Imagees
`sudo docker images`

### Remove Docker Images
`sudo docker rmi 45458imageid57459
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
`sudo docker stop 75498conarinerid8547
`sudo docker stop nameofcontainer`

### Remove Docker Container
`sudo docker rm 12364485containerid987459`
`sudo docker rm name`

### Remove all at once
`sudo docker container prune`

### Wordpress
`sudo docker run -p 8080:80 -v /home/swapkam/wordpress:/var/www/html -d --name my-wordpress-container wordpress`

`sudo docker ps -q -f "status=running" -f "label=com.docker.compose.project=<your-project-name>"`
`sudo docker inspect <container-id>`


# MongoDB
- sudo systemctl start mongod
- sudo systemctl status mongod
- sudo systemctl stop mongod
- sudo systemctl enable mongod
- sudo systemctl enable --now mongod
- sudo systemctl restart mongod

# Git
- git init
- git add .
- git commit -m "initial commit"
- git branch -M main
- git remote add origin https://github.com/swapkm/code.git
- git push -u origin main

## Apache2
`sudo systemctl start apache2`
`sudo systemctl status apache2`
# Xampp
`sudo /opt/lampp/manager-linux-x64.run`
`sudo /opt/lampp/lampp start`
`sudo /opt/lampp/lampp stop`
`sudo /opt/lampp/lampp restart`
`sudo /opt/lampp/lampp startftp`
`sudo /opt/lampp/lampp status`

## Apache2
- sudo systemctl start apache2
- sudo systemctl stop apache2
- sudo systemctl enable apache2
- sudo systemctl disable apache2


