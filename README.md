# Funcionamiento de la aplicación

## Puertos de funcionamiento

- APIRest → Puerto 8081

## Como ejecutar la aplicación

1. Abrir el proyecto que contiene el backend y ejecutar la clase *RestServiceApplication*
2. docker build -t rest-service .
3. docker run  -p 8081:8081 --net bridge --name Rest-Service rest-service
