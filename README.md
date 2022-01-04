# Funcionamiento de la aplicación

## Puertos de funcionamiento

- APIRest → Puerto 8081
- Frontend con Vaadin → Puerto 8080

## Como ejecutar la aplicación

1. Abrir el proyecto que contiene el backend y ejecutar la clase *RestServiceApplication*
2. Abrir el proyecto que contiene el frontend
3. Crear una nueva configuración de ejecución e introducir el comando
    
    ```jsx
    jetty:run
    ```
    
4. Ejecutar ambas aplicaciones y abrir [http://localhost:8080](http://localhost:8080)

## Implementaciones en la versión 2.0

### Frontend

- Pestaña Usuarios
    - Se desplegará un formulario para añadir un nuevo usuario al pulsar el botón "AÑADIR USUARIO".
    - Se podrá modificar un usuario desde el grid de usuarios
    - Se comprobará si un usuario puede ser eliminado o no en función de los préstamos asosciados
- Pestaña Equipos
    - Se abrirá una ventana con la información completa del equipo seleccionado
- Pestaña Préstamos
    - Se desplegará un formulario para añadir un nuevo préstamo al pulsar el botón "AÑADIR PRÉSTAMO".
    - Se podrá modificar un préstamo desde el grid de préstamos
- Creación de clases para los métodos que gestionan las peticiones PUT, POST, GET y DELETE

### Backend

- Implentación de Testing con JUnit 4