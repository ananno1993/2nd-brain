
### **Installing MySQL on Ubuntu**

1. Update the package index:
       
    `sudo apt update`
    
2. Install MySQL server:
    
    `sudo apt install mysql-server`
    
3. Secure the MySQL installation (set root password and other security options):
    
    `sudo mysql_secure_installation`
    
4. Check MySQL service status:
    
    `sudo systemctl status mysql`
    
5. Start MySQL service:
    
    `sudo systemctl start mysql`
    
6. Enable MySQL to start on boot:
        
    `sudo systemctl enable mysql`
    

---

### **MySQL Client Commands**

1. Login to MySQL as root user:

    `sudo mysql -u root -p`
    
2. Login to MySQL as a specific user:
    
    `mysql -u username -p`
    
3. Show all databases:
    
    `SHOW DATABASES;`
    
4. Select a database:
        
    `USE database_name;`
    
5. Show all tables in a database:

    `SHOW TABLES;`
    
6. Create a new database:
    
    `CREATE DATABASE database_name;`
    
7. Drop a database:

    `DROP DATABASE database_name;`
    
8. Create a new table:
   
    `CREATE TABLE table_name (     column1 datatype,     column2 datatype,     ... );`
    
9. Show table structure:

    `DESCRIBE table_name;`
    
10. Insert data into a table:
    
    `INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);`
    
11. Select data from a table:

    `SELECT * FROM table_name;`
    
12. Update data in a table:
    
    `UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;`
    
13. Delete data from a table:
   
    `DELETE FROM table_name WHERE condition;`
    
14. Drop a table:
    
    `DROP TABLE table_name;`
    

---

### **User Management**

1. Create a new user:
    
    `CREATE USER 'username'@'host' IDENTIFIED BY 'password';`
    
2. Grant privileges to a user:
    
    `GRANT ALL PRIVILEGES ON database_name.* TO 'username'@'host';`
    
3. Show all users:

    `SELECT User, Host FROM mysql.user;`
    
4. Revoke privileges from a user:
        
    `REVOKE ALL PRIVILEGES ON database_name.* FROM 'username'@'host';`
    
5. Delete a user:
   
    `DROP USER 'username'@'host';`
    

---

### **Backup and Restore**

1. Backup a database:

    `mysqldump -u username -p database_name > backup.sql`
    
2. Restore a database:

    `mysql -u username -p database_name < backup.sql`
    

---

### **MySQL Configuration**

1. Edit MySQL configuration file:

    `sudo nano /etc/mysql/mysql.conf.d/mysqld.cnf`
    
2. Restart MySQL service after configuration changes:

    `sudo systemctl restart mysql`
    

---

### **Common Troubleshooting Commands**

1. Show MySQL error log:
   
    `sudo tail -f /var/log/mysql/error.log`
    
2. Check MySQL status:

    `sudo systemctl status mysql`
    
3. Check MySQL logs for issues:

    `sudo journalctl -u mysql.service`
    
4. Check disk space:
   
    `df -h`
    

---

### **Miscellaneous MySQL Commands**

1. Show current MySQL version:
    
    `mysql --version`
    
2. Show current MySQL variables:

    `SHOW VARIABLES;`
    
3. Exit MySQL:
  
    `EXIT;`

