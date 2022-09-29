# amigosservices
TOURISTS-HUB-SERBIA
WEB APPLICATION

[Adedotun Olasunkanmi Ogundare](https://github.com/dotun-ogundare)

<h1>Project Description</h1>

This is a project conducted by Dotun Ogundare (2021/2022 academic year) enrolled in masters of Software Engineering & Information Technologies at the Faculty of Technical Sciences of the University of Novi Sad. The project is the practical requirement for the Software Configuration Management [Course](https://github.com/vladaindjic/SCM-exchange-students#the-project-specification) which has exposed the students to the essential tools, concepts and state-of-art technologies for maintaining web application life cycle especially for a cloud-native application. This project is named the ‘Serbia-tourist-hub’ and it is an online platform where tourists in Serbia can visit and see all the tourist attractions and events around them. This helps to solve the curiosity that lies within people who arrive in Serbia in their first week. The developers, being foreigners in Serbia, had a fair share of same curiosity in their first week at Novi Sad in their attempts to explore the ‘European Capital of Culture.’ As such, they grapple with the plethora of generic and hackneyed information that internet offers. Away from the cliché of asking native Serbians around, the project is motivated by the need to build a solution that will guide tourists in Serbia. As such, it is optimized for Serbia with the goal of showcasing an exhaustive tourist documentation of arts, culture and tourism in the country. Aside being at the centerpiece of the two world wars, Serbia is a country of rich culture and heritage with significant historical relevance to global politics and scramble for political power. The [Serbia-tourist-hub](https://github.com/vladaindjic/SCM-exchange-students/blob/master/SPEC.md) will be a go-to platform for anybody arriving Serbia as educationist, researcher, student, or tourist. 

The project is being supervised by [Vladimir Inđić](https://github.com/vladaindjic) under the ultimate supervision of Professor Igor

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


![message queue](https://user-images.githubusercontent.com/50335434/193032886-2b3b78fa-dc12-43aa-9200-7e4151c67bf5.png)

 

