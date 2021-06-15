##Instalar MariaDB en MacOS e integrarlo con DBeaver

Paso 1 - Homebrew update
Paso 2 - Instalar MariaDB mediante Homebrew -> brew install mariadb
Paso 3 - Definir Usuario mysql -u root -p
Pago 4 - en caso de presentar falla aplicar el siguiente comando
comando: sudo mysql

-- for MySQL
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';

-- for MariaDB
ALTER USER 'root'@'localhost' IDENTIFIED VIA mysql_native_password USING PASSWORD('root');

#Para crear Base de Datos:
comando: CREATE DATABASE storage;
comando para visaulizar bases de datos: SHOW DATABASES;

#Eliminar Bases de Datos
comando: DROP DATABASE storage;

#Ingresar a una BD
comando: USE storage:
