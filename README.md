# TASK_1
Exploring the  SQL_Injection and XSS attacks 
To setup DVWA:
1) git clone https://github.com/digininja/DVWA.git to /var/www/html directory, this directory allow the user to run a web application lon local machine(directory to host a web application in linux).

2) change the file permission of the DVWA directory using the follwing command
chmod -R 777 DVWA
3) go to the DVWA folder and to config folder
4) now make a copy of the config.inc.php.dist file and rename it to config.inc.php and edit it with the text editor
5) change the user and password ex: admin : password
6) start the apache2 service: systemctl start apache2
7) start mysql : systemctl start mysql
8) mysql -u root -p press enter 2 times
9) now create the user account for the mysql database use the following commands \
   a) create database dvwa;
   b) create user 'admin'@'127.0.0.1' identified by 'password';
   c)grant all privileges on dvwa.* to 'admin'@'127.0.0.1';
10) now go to /etc/php/yourphpversion/
11) and edit the php.ini file and search for the fopen
12) now replace the off with on value in allow_url_fopen and allow_url_include both these parameters
13) now restart the apache2 server and go to your browser and type localhost:4040 or 127.0.0.1:4040
14) now login with the user name and password you created, In this case its username: admin and password: password
15) Now you can test the DVWA and practice your skills 
  
