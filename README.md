# SpringBoot---Microservices
Department Service :   This is one of the microservice which will able to POST and GET the request.

User Service :  This is other microservice which will able to POST and GET the request and also communicate with Deparment microservice.

API - GATEWAY : All the microservices are connected through the API-GATEWAY. Infact, all the microservoces are connected through the API-GATEWAY.

SERVICE - REGISTRY: All the microservice are register on the local server. In this case we are using Eureka Server. So we have to give definition of Eureka in all our microiservices.

   We have to create Eureka Dashboard as well so that we can monitor all our micoservices and check which of the microsevices are UP and which are the down.
   
HYSTRIX - DASHBOARD : If we have n number of microservices then it is very difficult to minitor all the microservices through the Eureka Server.That's Why Hystrix dashboard shows the graphical representation of the microservices. All the microservices are responding 100% or not, it will monitor these types of things.

CLOUD-CONFIG-SERVER : If same things(Same code structure) are repeated in all our microservices(just like Eureka server definition in this case because we have to register all our microservices in the Eureka Server). Then we will create a github repositry having same code and pass the URL in our application.yml file.

  And if anything changes have to be done in that code structure then we will simply change the github repo and it will change all our microservoces as well. 
