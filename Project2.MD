#   LEMP STACK IMPLEMENTATION - PROJECT 2

*Step 1 – Installing the Nginx Web Serveri*

`sudo apt update`

![atp-update](./images/apt-update.png)

`sudo apt install nginx`

![apt=install-nginx](./images/apt-install-nginx.png)

`sudo systemctl status nginx`

![systemctl-status-nginx](./images/systemctl-status-nginx.png)

`curl http`

![curl-http](./images/curl-http.png)

`nginx website`

![nginx-website](./images/nginx-website.png)

# STEP 2 — INSTALLING MYSQL

`sudo apt install mysql-server`


![mysql-server](./images/mysql-server.png)

`sudo mysql`


![sudo-mysql](./images/sudo-mysql.png)

`sudo mysql_secure_installation`

![mysql-secure-installation](./images/mysql-secure-installation.png)

# STEP 3 – INSTALLING PHP

`sudo apt install php-fpm php-mysql`

![php-mysql](./images/php-mysql.png)

# STEP 4 — CONFIGURING NGINX TO USE PHP PROCESSOR
`sudo mkdir /var/www/projectLEMP`
`sudo chown -R $USER:$USER /var/www/projectLEMP`
`sudo nano /etc/nginx/sites-available/projectLEMP`
`sudo ln -s /etc/nginx/sites-available/projectLEMP /etc/nginx/sites-enabled/`

![sudo-in-s](./images/sudo-in-s.png)

`sudo nginx -t`
`sudo unlink /etc/nginx/sites-enabled/default`
`sudo systemctl reload nginx`
`sudo echo`

![sudo-echo](./images/sudo-echo.png)

# STEP 5 – TESTING PHP WITH NGINX
`sudo nano /var/www/projectLEMP/info.php`
`sudo rm /var/www/your_domain/info.php`

# STEP 6 – RETRIEVING DATA FROM MYSQL DATABASE WITH PHP (CONTINUED)
`sudo mysql`