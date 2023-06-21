# Ubuntu
Install filename.run
- chmod +x filenam*.run
- sudo ./filenam*.run
- unzip file.zip
- unzip file.zip -d myfolder
- zip -r my_archive.zip my_folder/
- zip -r archive-name.zip folder-name
- rm -r az - remove folder which contains files
- zip -r my_directory.zip /path/to/my_directory

### If want to rename directory
- mv oldfolder newfolder
- sudo dpkg -i filemane-*.deb

### Wordpress
- sudo docker run -p 8080:80 -v /home/swapkam/wordpress:/var/www/html -d --name my-wordpress-container wordpress

- sudo docker ps -q -f "status=running" -f "label=com.docker.compose.project=<your-project-name>"
- sudo docker inspect <container-id>


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

# Xampp
`sudo /opt/lampp/manager-linux-x64.run`
`sudo /opt/lampp/lampp start`
`sudo /opt/lampp/lampp stop`
`sudo /opt/lampp/lampp restart`
`sudo /opt/lampp/lampp startftp`
`sudo /opt/lampp/lampp status`

## Apache2
- sudo systemctl start apache2
- sudo systemctl status apache2
- sudo systemctl stop apache2
- sudo systemctl enable apache2
- sudo systemctl disable apache2


