# TP Microservices : Eureka, Client, Voiture, Gateway

Projets Maven independants (Spring Boot 3.3.5, Spring Cloud 2023.0.3, Java 17+).
Utiliser le JDK 21 (Temurin) dans IntelliJ.

Ordre de lancement :
1. eureka-server  (8761)
2. service-client (8088)
3. service-voiture (8089)
4. gateway (8888)

Attendre environ 30 secondes apres le demarrage avant de tester via la Gateway.

Tests :
- http://localhost:8761
- http://localhost:8088/clients , /client/1
- http://localhost:8089/voitures , /voitures/1 , /voitures/client/1
- http://localhost:8888/clients , /client/1 , /voitures
- http://localhost:8888/SERVICE-CLIENT/clients , /SERVICE-VOITURE/voitures
