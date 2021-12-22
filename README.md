# IdeaCat Tutorials 

##### usage of mysqldump for exporting database .sql file
# mysqldump

MySQL brings a simple way to export a database from the command line to a specified folder with one simple command.

First, you have to ensure you're connected to the database and you have to run:
```
mysql -u user -p
```
And next, you have to introduce the password of the database user.
```
Enter password:
```

Next check which database you want to export running the following in the MySQL console:
```
mysql> SHOW DATABASES;
```

The output should look like this.

```
+--------------------+
| Database           |
+--------------------+
| forge              |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)

```
Now you can choose the name of the database you want to export and after pressing
``` CTR + Z ``` 
to exit the MySQL console run the mysqldump command.


```
mysqldump -u username -p databasename > filename.sql
```

This command will generate for you a fresh copy of your MySQL database into the current folder.



This tutorial was delivered to you by ["IdeaCat"](https://ideacat.ro/).



