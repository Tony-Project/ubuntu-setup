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

step 4 -
1.	sudo apt-get update
 
2.	sudo apt install xrdp
 
3.	sudo apt-get install xserver-xorg-core
 
4.	sudo apt-get install xorgxrdp
 
5.	nano /etc/polkit-1/localauthority.conf.d/02-allow-colord.conf
 
6.	Copy the polkit
 
polkit.addRule(function(action, subject) {
if ((action.id == “org.freedesktop.color-manager.create-device” || action.id == “org.freedesktop.color-manager.create-profile” || action.id == “org.freedesktop.color-manager.delete-device” || action.id == “org.freedesktop.color-manager.delete-profile” || action.id == “org.freedesktop.color-manager.modify-device” || action.id == “org.freedesktop.color-manager.modify-profile”) && subject.isInGroup(“{group}”))
{
return polkit.Result.YES;
}
});
 
7.	sudo ufw allow 3389/tcp
 
8.	sudo /etc/init.d/xrdp restart
 
9.	sudo systemctl status xrdp
 
10.	sudo systemctl enable xrdp
 
11.	Get IP address 
 
12.	Log out of ubuntu




Node & Ionic Setup :

sudo apt update
sudo apt install nodejs
nodejs -v
sudo apt install npm

sudo npm install -g @angular/cli
sudo npm i -g @adonisjs/cli
sudo npm install -g @ionic/cli

npm install -g ionic cordova
