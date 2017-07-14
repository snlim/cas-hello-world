# Cas Hello World Project

This project shows how to integrate CAS 3.4.10 with Spring Security 3. It verify and authenticate credentials using Basic Authentication.

## Run

To run the project                                                               
```
mvn jetty:run
```

To access the project
```
http://localhost:8080/hello-world-cas/diagnostic.html
```

To access the CAS
```
http://localhost:8080/cas
```

To login, only the 'admin' and 'abc' are authorized to access the disgnostic page. 
The user that carry other same netId and password are able to pass through the CAS authentication, but will not be granted any authority to access the diagnostic page. 
Refer to "src\main\webapp\WEB-INF\security-context.xml" under "userService" bean to add more authorized users. 
```
netId: admin
password: admin   
```
