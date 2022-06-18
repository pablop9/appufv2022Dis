# Funcionamiento de la aplicación

## Puertos de funcionamiento

- APIRest → Puerto 8081

## Como ejecutar la aplicación

1. Crear la red privada de docker de tipo bridge
   ```jsx
    docker network create -d bridge --subnet 192.168.0.0/16 conexion-front-back
    ```
2. Generar imagen del contenedor
    ```jsx
    docker build -t rest-service .
    ```
3. Ejecutar contenedor
    ```jsx
    docker run  -p 8081:8081 --net conexion-front-back --ip 192.168.1.1 --name Rest-Service rest-service
    ```
