# ubuntu-setup
step 1 - Apache, Mysql, Php
*https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-20-04
*ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '<password>';
*FLUSH PRIVILEGES;
  
step 2 - phpmyadmin
*https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-20-04
*sudo ln -s /etc/phpmyadmin/apache.conf /etc/apache2/conf-available/phpmyadmin.conf
*sudo a2enconf phpmyadmin.conf
*sudo systemctl restart apache2

step 3 - 
*https://www.tecmint.com/set-display-screen-resolution-in-ubuntu/amp/
*https://itsfoss.com/click-to-minimize-ubuntu/
