## Day 7 : Fundamental Cloud Computing and Database Management

### Appserver for deploying Database

### Gateaway for deploying Frontend, Backend, and Web Server

![Server](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/01.%20ServerGCP.png)

### Create new user for all of your server

### The server only can login with SSH-KEY without using password at all

![SSH](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/02.%20User&SSH.png)

### Deploy database MySQL

- Setup secure_installation

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/03.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/04.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/05.%20DeployDatabase.png)

- Add password for root user

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/06.%20DeployDatabase.png)

- Create new user for MySQL

- Create new database

- Create privileges for your new user so they can access the database you created

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/07.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/08.%20DeployDatabase.png)

- Dont forget to change the MySQL bind address on /etc/mysql/mysql.conf.d/mysqld.cnf

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/09.%20DeployDatabase.png)

![Database](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/10.%20DeployDatabase.png)

### Role Based

- Create new database call demo and make some dummy table call transaction

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/11.%20RoleBased.png)

- Create a 2 role with the name admin, and guest that will be used to see and manage the 'transaction' table.

- Give SELECT, INSERT, UPDATE, and DELETE access rights to the transaction table for the admin role you just created. and only give SELECT access to guest.

- Create a new user with the username your_name and password your_password. Add the user to the admin role.

- Create a new user with the username guest and password guest. Add the user to the guest role.

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/12.%20RoleBased.png)

- Test all of your user

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/13.%20RoleBased.png)

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/14.%20RoleBased.png)

![Role](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/15.%20RoleBased.png)

### Remote User

- Try to remote your database from your local computer with mysql-client

![Remote](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/16.%20RemoteUser.png)

### Deploy Wayshub-Backend

- Clone wayshub backend application

- Use Node Version 14

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/17.%20DeployBackend.png)

- Dont forget to change configuration on dumbflix-backend/config/config.json and then adjust it to your database.

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/18.%20DeployBackend.png)

- Install sequelize-cli

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/19.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/20.%20DeployBackend.png)

- Running migration

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/21.%20DeployBackend.png)

- Hasil migration

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/22.%20DeployBackend.png)

- Deploy apllication on Top PM2

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/23.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/24.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/25.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/26.%20DeployBackend.png)

- Konfigurasi web-server

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/27.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/28.%20DeployBackend.png)

![backend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/29.%20DeployBackend.png)

### Deploy Wayshub-Frontend

- Clone wayshub frontend application

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/30.%20DeployFrontend.png)

- Use Node Version 14

- Dont forget to change configuration on src/config/api.js and then adjust it to backend url.

- Deploy frontend apllication on Top PM2

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/31.%20DeployFrontend.png)

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/32.%20DeployFrontend.png)

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/33.%20DeployFrontend.png)

- Konfigurasi web-server

![frontend](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/34.%20DeployFrontend.png)

#### Hasil Akhir

- Pemasangan SSL

![SSL](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/35.%20SSL.png)

![SSL](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/36.%20SSL.png)

![SSL](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/37.%20SSL.png)

- Output

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/38.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/39.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/40.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/41.%20Hasil.png)

![Hasil](https://github.com/Bagusylyto/devops28-dumbways-bagus/blob/main/Task7/42.%20Hasil.png)
