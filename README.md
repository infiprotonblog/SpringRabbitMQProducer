# SpringRabbitMQPublisher
1. Advanced Message Queuing Protocol (AMQP) is a platform-neutral, wire-level protocol for message-oriented middleware.
2. The Spring AMQP project applies core Spring concepts to the development of AMQP-based messaging solutions. 
3. Spring Boot offers several conveniences for working with AMQP through RabbitMQ.
4. RabbitMQ is a lightweight, reliable, scalable, and portable message broker based on the AMQP protocol. 
5. Spring uses RabbitMQ to communicate through the AMQP protocol.

# Requirements
1. Java - 1.8.x
2. Maven - 3.x.x

# We need to install and setup RabbitMQ to run the application 
1. RabbitMQ is built on top of Erlang, we will first need to install Erlang. 
2. Got to the Erlang downloads page and download the erlang binary file for windows which is an executable.
3. Next run the binary file downloaded and install erlang on your machine.
4. Go to RabbitMQ downloads page and download RabbitMQ installation.
5. Go to the RabbitMQ Server Location and use the command as follows- 'rabbitmq-server start'
6. Next install the RabbitMQ plugin which will give use the RabbitMQ Management Console which is accessible using the browser. 
7. For this use the command as follows- 'rabbitmq-plugins.bat enable rabbitmq_management'
8. Next go to 'localhost:15672'. We will see the RabbitMQ console. The default username and password is 'guest'.

# Dependency required 
Add the 'spring-boot-starter-amqp' dependency.

# Steps to Run the application
1. Type $ mvn spring-boot:run from the root project directory to start the application.
2. We can browse the application at 'http://localhost:15672/#/queues' and check the new queues and new connections.

Next to receive the message we need to have consumer configuration. (clone 'https://github.com/infiproton/SpringRabbitMQSubscriber')




