`docker run -d --name mariadb -e MARIADB_ROOT_PASSWORD=Esc-F1F2F3 -e MARIADB_USER=swapkam -e MARIADB_PASSWORD=Esc-F1F2F3 -e MARIADB_DATABASE=nextcloud_db -p 3306:3306 -v mariadb_data:/var/lib/mariadb mariadb:latest`

`docker run -d --name mariadb --network bridge -e MARIADB_ROOT_PASSWORD=Esc-F1F2F3 -e MARIADB_DATABASE=nextcloud_db -e MARIADB_USER=swapkam -e MARIADB_PASSWORD=Esc-F1F2F3 -p 3306:3306 -v mariadb_data:/var/lib/mysql mariadb:latest`

`docker run -d --name nextcloud --network bridge -p 8080:80 -v nextcloud_data:/var/www/html/data nextcloud:latest`

`docker run -d --name nextcloud --network bridge -p 8080:80 -v nextcloud_data:/var/www/html/data -e MYSQL_DATABASE=nextcloud_db -e MYSQL_USER=swapkam -e MYSQL_PASSWORD=Esc-F1F2F3 -e MYSQL_HOST=mariadb nextcloud:latest`

`docker run -d --name phpmyadmin --network bridge -p 8081:80 -e PMA_HOST=mariadb -e PMA_USER=swapkam -e PMA_PASSWORD=Esc-F1F2F3 -v phpmyadmin_data:/sessions phpmyadmin:latest`