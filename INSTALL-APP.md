
![SCREEN1](screen-01.jpg)

* From the current URL navigate to **/install/install.php** through the browser's address bar. Here you will find the installers welcome page. Klick on **Start installation**.

![SCREEN2](screen-02.jpg)

* On the next page a form for configuring installation paths will appear. 
* From the current URL navigate to **/install/install.php** through the browser's address bar. Here you will find the installers welcome page. 
Update in the database settings the password as you specified in the App installation screen and 
make sure to check **Create database tables** and click **Apply**!

![SCREEN3](screen-03.jpg)
![SCREEN2](screen-03.jpg)

* After the installation has succeeded, another screen with two links will appear. 
Click on **Delete the ENABLE_INSTALL_TOOL if possible**.

![SCREEN4](screen-04.jpg)
![SCREEN3](screen-04.jpg)

* The setting for forcing the installation will now be deleted and the application is ready for usage. Click on **Configure more settings. Default login: admin/admin**.

![SCREEN5](screen-05.jpg)
![SCREEN4](screen-05.jpg)

* You will now see the login screen. Please use username **admin** and password **admin** to log in.

![SCREEN6](screen-06.jpg)
![SCREEN5](screen-06.jpg)

* That's it! You have successfully installed SeedDMS and are ready for managing your documents with it!

![SCREEN7](screen-07.jpg)
![SCREEN6](screen-07.jpg)


## Backup instructions
* Backup the database App directory, replace APPID with the id (subdomain) of the installed app. 
        /opt/bibbox/application-instance/APPID-app-seeddms
        
* Backup the data directory 
    
        /opt/bibbox/application-instance/APPID-app-seeddms/data/var/www/seeddms51x
        
* Backup the mysql database with the command
       
       docker exec  APPID-seeddms-db /usr/bin/mysqldump -u root --password='YOURROOTPASSWORD' seeddms > /home/vmadmin/seeddmsbackup.sql
   if you forgot the database root password, you can lookup it in the docker-compose file. 
   
        /opt/bibbox/application-instance/APPID-app-seeddms/docker-compose.yml
## After the installation
Have a nice ride with the new Admins youngtimer.
