
### 1. **Installation Commands**

To install MongoDB on Ubuntu, follow these commands:

**Update the local package database:**

`sudo apt update`

**Install MongoDB:**

`sudo apt install -y mongodb`

**Verify the installation:**

`mongod --version`

### 2. **Starting and Stopping MongoDB Service**

**Start MongoDB service:**

`sudo systemctl start mongodb`

**Stop MongoDB service:**

`sudo systemctl stop mongodb`

**Restart MongoDB service:**

`sudo systemctl restart mongodb`

**Check MongoDB service status:**

`sudo systemctl status mongodb`

**Enable MongoDB to start on boot:**

`sudo systemctl enable mongodb`

**Disable MongoDB from starting on boot:**

`sudo systemctl disable mongodb`

### 3. **MongoDB Shell Commands**

**Start the MongoDB shell:**

`mongo`

**Show available databases:**

`show databases`

**Switch to a database:**

`use <dbname>`

**Show collections in the current database:**

`show collections`

**Create a new collection:**

`db.createCollection("collectionName")`

**Insert a document into a collection:**

`db.collectionName.insert({name: "John", age: 30})`

**Find documents in a collection:**

`db.collectionName.find()`

**Query documents in a collection:**

`db.collectionName.find({name: "John"})`

**Update a document in a collection:**

`db.collectionName.update({name: "John"}, {$set: {age: 31}})`

**Delete a document from a collection:**

`db.collectionName.remove({name: "John"})`

**Drop a collection:**

`db.collectionName.drop()`

**Drop a database:**

`db.dropDatabase()`

**Exit the MongoDB shell:**

`exit`

### 4. **Backup and Restore Commands**

**Create a backup using `mongodump`:**

`mongodump --out /path/to/backup/`

**Restore from a backup using `mongorestore`:**

`mongorestore /path/to/backup/`

### 5. **Security Commands**

**Enable authentication:**

`sudo nano /etc/mongodb.conf # Add the following line to enable authentication: security:     authorization: "enabled"`

**Create a user in the MongoDB shell:**

`use admin db.createUser({     user: "admin",     pwd: "password",     roles: [{role: "userAdminAnyDatabase", db: "admin"}] })`

**Authenticate as a user:**

`db.auth("admin", "password")`

### 6. **Managing MongoDB Logs**

**View MongoDB logs:**

`sudo tail -f /var/log/mongodb/mongod.log`

### 7. **Upgrade MongoDB**

**Upgrade MongoDB:**

`sudo apt update sudo apt upgrade mongodb`

### 8. **Remove MongoDB**

**Remove MongoDB from the system:**

`sudo apt purge mongodb sudo apt autoremove`


