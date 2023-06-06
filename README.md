# MICROSERVICE FOR SENDING EMAIL WITH SPRING AND JAVA

## About the project

Email sending microservice through Postman.

### request body via postman

{
    "ownerRef": "name or ID generic",
    "emailFrom": "your-email@gmail.com",
    "emailTo": "email-teste@gmail.com",
    "subject": "message",
    "text": "Title of message",
}

## Starting project

1. Dependencies required for the project.

- Lombok
- Spring Date JPA
- Spring Web
- Validation
- Spring Mail Sender
- MySQL Driver

2. Configuration to connect with MySQL database.

server.port=8080

spring.datasource.url=jdbc:mysql://localhost:3306/emails
spring.datasource.username='name of database'
spring.datasource.password='password'
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update

spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

3. Configuration to connect with Gmail.

spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username='your e-mail'
spring.mail.password='16 character code'
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true

3. 1. Configuring the 16-character code for connecting to Gmail

1. Manage your Google account
2. Security
3. in the box "How do you sign in to Google"
4. two-step verification
5. Enter your Google email password
6. At the bottom of the page, "App Passwords"
7. generate password