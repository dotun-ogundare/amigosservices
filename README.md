# amigosservices
TOURISTS-HUB-SERBIA
WEB APPLICATION

[Adedotun Olasunkanmi Ogundare](https://github.com/dotun-ogundare)

<h1>Project Description</h1>

This is a project conducted by Dotun Ogundare (2021/2022 academic year) enrolled in masters of Software Engineering & Information Technologies at the Faculty of Technical Sciences of the University of Novi Sad. The project is the practical requirement for the Software Configuration Management 

The goal of the project is to further demonstrate the knowledge of Software Configuration Management tools that was learnt in the academic year.

Technical Overview
 
 It follows a microservices based architecture created for the purpose of verifying the history of a customer. It comprises of three services
 
 Customer- interacts with the database for customer records and sends to the Fraud service
 Fraud - the fraud service checks the customer records and returns teh status of the customer as either having fraudulent history or not
 Notification - handles the notification of the customer service using twilio API
 
 In addition to the services, Eureka server, API Gateway are also implemented as services. Zipkin is used for distributed tracing, Rabbit MQ is used for message queue to manage asynchronous commmunication between customer service and notification service
 
The project is implemented with java using Maven as built tool. 
The backend is designed using spring boot. 
The backend are bundled into a jar and built into a docker image which is pushed into docker hub using Jib
The docker-compose.yml file references the particular repository of the images created. 

CICD
Github is used as the Version Control System for managing updates and versioning of the application the application


![Capture](https://user-images.githubusercontent.com/50335434/193033075-155be2c6-040a-4360-8842-574c852c4b62.PNG)
 

