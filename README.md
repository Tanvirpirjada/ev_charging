# ev_charging
ev charging stati_springboot_applicatio
 
# Weekly_test_api

In this project we build ev chrging station.

# framework and languges
* Springboot framework is used
* Java is Used for code

# Data flows

* UI(postman or localhost 8080 made requests)

# 1 Cotroller
* Cotroller -> requestcome from ui and  execute mathod in cotroller based on end points. In controller various mathods are available Ex

station -> create/post: http://localhost:8081/savestation

           Getstation: http://localhost:8081/getstation(requestparam=station_id)

            Updatestation: http://localhost:8081/Updatestation/{station_id}

            Deletestation: http://localhost:8081/savestation (requestparam =station_id)
           


* form controller service methods are call where our main buisness logic is wriiten

# 2 service

* the methods are called and its get data from databse with help of repository layer

# 3 Repository 
repository layes is help to connect with database 

# used databse
->Mysql

# data Structure
->  ArrayList

# Apllication.properties
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url = jdbc:mysql://localhost:3306/ev_stationdb
spring.datasource.username = root
spring.datasource.password = Tanvir@786
spring.jpa.show-sql = true
spring.jpa.hibernate.ddl-auto = update
spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL5Dialect
server.port=8081

