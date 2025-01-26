### **Basic Apache2 Commands**

1. **Start Apache2 service**

    `sudo systemctl start apache2`
    
2. **Stop Apache2 service**
  
    `sudo systemctl stop apache2`
    
3. **Restart Apache2 service**

    `sudo systemctl restart apache2`
    
4. **Reload Apache2 service (without full restart)**

    `sudo systemctl reload apache2`
    
5. **Check Apache2 service status**
  
    `sudo systemctl status apache2`
    
6. **Enable Apache2 service to start on boot**

    `sudo systemctl enable apache2`
    
7. **Disable Apache2 service from starting on boot**

    `sudo systemctl disable apache2`
    
8. **Check Apache2 version**

    `apache2 -v`
    
9. **Check configuration syntax**
 
    `sudo apache2ctl configtest`
    
10. **Test Apache2 configuration**
  
    `sudo apache2ctl -t`
    
11. **Start Apache2 in the foreground (useful for debugging)**

    `sudo apache2ctl -D FOREGROUND`
    
12. **Stop Apache2 in the foreground**

    `sudo apache2ctl stop`
    
13. **Display help for Apache2**

    `apache2ctl -h`
    

### Apache2 Modules Management

1. **Enable a module**

    `sudo a2enmod <module_name>`
    
2. **Disable a module**
  
    `sudo a2dismod <module_name>`
    
3. **List all enabled modules**

    `apache2ctl -M`
    

### Apache2 Sites Management

1. **Enable a site**

    `sudo a2ensite <site_config_file>`
    
2. **Disable a site**

    `sudo a2dissite <site_config_file>`
    
3. **List enabled sites**

    `ls /etc/apache2/sites-enabled/`
    
4. **List available sites**

    `ls /etc/apache2/sites-available/`
    

### Apache2 Configuration File Management

1. **Edit Apache2 main configuration file**

    `sudo nano /etc/apache2/apache2.conf`
    
2. **Edit Apache2 virtual hosts configuration**

    `sudo nano /etc/apache2/sites-available/000-default.conf`
    
3. **Edit security settings for Apache2**
 
    `sudo nano /etc/apache2/conf-available/security.conf`
    

### Logs Management

1. **View Apache2 error log**

    `sudo tail -f /var/log/apache2/error.log`
    
2. **View Apache2 access log**

    `sudo tail -f /var/log/apache2/access.log`
    

### Apache2 Service Status

1. **Get the Apache2 service status (including active/inactive)**
 
    `sudo systemctl is-active apache2`
