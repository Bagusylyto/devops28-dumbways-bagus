## Day 7 : Fundamental Cloud Computing and Database Management

### Appserver for deploying Database

### Gateaway for deploying Frontend, Backend, and Web Server

![Server](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/01.%20ServerGCP.png)

### Create new user for all of your server

### The server only can login with SSH-KEY without using password at all

![SSH](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/02.%20User&SSH.png)

### Deploy database MySQL

- Setup secure_installation

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/03.%20DeployDatabase.jpg)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/04.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/05.%20DeployDatabase.png)

- Add password for root user

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/06.%20DeployDatabase.png)

- Create new user for MySQL

- Create new database

- Create privileges for your new user so they can access the database you created

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/07.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/08.%20DeployDatabase.png)

- Dont forget to change the MySQL bind address on /etc/mysql/mysql.conf.d/mysqld.cnf

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/09.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/10.%20DeployDatabase.png)

### Role Based

- Create new database call demo and make some dummy table call transaction

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/11.%20RoleBased.png)

- Create a 2 role with the name admin, and guest that will be used to see and manage the 'transaction' table.

- Give SELECT, INSERT, UPDATE, and DELETE access rights to the transaction table for the admin role you just created. and only give SELECT access to guest.

- Create a new user with the username your_name and password your_password. Add the user to the admin role.

- Create a new user with the username guest and password guest. Add the user to the guest role.

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/12.%20RoleBased.png)

- Test all of your user

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/13.%20RoleBased.png)

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/14.%20RoleBased.png)

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/15.%20RoleBased.png)

### Remote User

- Try to remote your database from your local computer with mysql-client

![Remote](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/16.%20RemoteUser.png)

### Deploy Wayshub-Backend

- Clone wayshub backend application

- Use Node Version 14

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/17.%20DeployBackend.jpg)

- Dont forget to change configuration on dumbflix-backend/config/config.json and then adjust it to your database.

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/18.%20DeployBackend.png)

- Install sequelize-cli

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/19.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/20.%20DeployBackend.png)

- Running migration

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/21.%20DeployBackend.png)

- Hasil migration

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/22.%20DeployBackend.png)

- Deploy apllication on Top PM2

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/23.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/24.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/25.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/26.%20DeployBackend.png)

- Konfigurasi web-server

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/27.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/28.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/29.%20DeployBackend.png)

### Deploy Wayshub-Frontend

- Clone wayshub frontend application

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/30.%20DeployFrontend.png)

- Use Node Version 14

- Dont forget to change configuration on src/config/api.js and then adjust it to backend url.

- Deploy frontend apllication on Top PM2

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/31.%20DeployFrontend.png)

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/32.%20DeployFrontend.png)

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/33.%20DeployFrontend.png)

- Konfigurasi web-server

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/34.%20DeployFrontend.png)

#### Hasil Akhir

- Pemasangan SSL

![SSL](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/35.%20SSL.png)

![SSL](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/36.%20SSL.png)

![SSL](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/37.%20SSL.png)

- Output

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/38.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/39.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/40.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/41.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/images/42.%20Hasil.png)

- Website
  [wayshub](http://bagus.studentdumbways.my.id/)
