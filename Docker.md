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

### See All Docker Images
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

`sudo docker volune prune`


#### Portainer

`docker volume create portainer_data`

`docker run -d -p 9000:9000 -p 9443:9443 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest`

#### MariaDB

`docker run -d --name mariadb --network bridge --restart always -e MARIADB_ROOT_PASSWORD=Esc-F1F2F3 -e MARIADB_USER=swapkam -e MARIADB_PASSWORD=Esc-F1F2F3 -e MARIADB_DATABASE=nextcloud_db -p 3306:3306 -v mariadb_data:/var/lib/mysql mariadb:latest`

`docker exec -it mariadb /bin/bash`

`mariadb -u root -p`

`show databases;`

#### PHPMyAdmin

`docker run -d --name phpmyadmin --network bridge --restart always -p 3366:80 -e PMA_HOST=mariadb -e PMA_PASSWORD=Esc-F1F2F3 -v phpmyadmin_data:/var/lib/mysql/data phpmyadmin:latest`


#### NextCloud

`docker run -d --name nextcloud --network bridge --restart always -p 8080:80 -v nextcloud_data:/var/www/html nextcloud:latest`


### Pi-hole

`version: "3"

# More info at https://github.com/pi-hole/docker-pi-hole/ and https://docs.pi-hole.net/
services:
  pihole:
    container_name: pihole
    image: pihole/pihole:latest
    # For DHCP it is recommended to remove these ports and instead add: network_mode: "host"
    ports:
      - "53:53/tcp"
      - "53:53/udp"
      - "67:67/udp" # Only required if you are using Pi-hole as your DHCP server
      - "8000:80/tcp"
    environment:
      TZ: 'Asis/Kolkata'
      WEBPASSWORD: 'Esc-F1F2F3'
    # Volumes store your data between container upgrades
    volumes:
      - './etc-pihole:/etc/pihole'
      - './etc-dnsmasq.d:/etc/dnsmasq.d'
    #   https://github.com/pi-hole/docker-pi-hole#note-on-capabilities
    cap_add:
      - NET_ADMIN # Required if you are using Pi-hole as your DHCP server, else not needed
    restart: unless-stopped
`