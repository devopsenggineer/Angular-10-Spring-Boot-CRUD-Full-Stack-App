#  Angular-10-Spring-Boot-CRUD-Full-Stack-App

# Steps for running  Angular-10-Spring-Boot-CRUD-Full-Stack-App project

# Deploy/Install mysql-5 database docker contaienr
sudo docker run -d --name mysql_db -e  "MYSQL_ROOT_PASSWORD=123456" -p 3306:3306 mysql:5

# Go inside mysql_db container
sudo docker exec -it mysql_db bash

# Run below command inside mysql_db container and enter root user password when prompted
mysql -u root -p

# Now create "employee_management_system" mysql database from mysql prompt
CREATE DATABASE employee_management_system;

# Now enter  "employee_management_system" created database
use employee_management_system;

# Now run below sql query from mysql prompt to employees table, it will throw error this time
select * from employees;


# Git clone this repo
git clone https://github.com/sysadmin-imran/Angular-10-Spring-Boot-CRUD-Full-Stack-App.git

# Open springboot-backend project inside  cloned "Angular-10-Spring-Boot-CRUD-Full-Stack-App" directory in any IDE like Intellij

# Run the the file "SpringbootBackendApplication.java" under "springboot-backend/src/main/java/com/javaguides/springbootbackend" folder

# Now Go inside Angular-10-Spring-Boot-CRUD-Full-Stack-App/angular-frontend/
cd Angular-10-Spring-Boot-CRUD-Full-Stack-App/angular-frontend/

# Install node modules
npm install

# start Angular app
npm start 
OR
ng serve

