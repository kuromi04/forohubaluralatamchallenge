# ForoHub: API REST para un Foro

![4951974800276958671](https://github.com/user-attachments/assets/7dda2a89-af0f-4f52-a042-c23457767447)

## � Descripción del Proyecto

ForoHub es una API RESTful diseñada para replicar la funcionalidad de un foro de discusión. Este proyecto forma parte de la certificación en back-end con especialidad en Spring Boot en Alura Latam. Permite la gestión de tópicos y autores, proporcionando un espacio para la creación, consulta, actualización y eliminación de estos elementos.

En Alura Latam, el foro es un espacio vital donde los estudiantes resuelven dudas y comparten conocimientos. ForoHub busca replicar este entorno de colaboración y aprendizaje, centrando sus funcionalidades en los tópicos del foro.

## � Tecnologías Utilizadas

- **Java**
- **Spring Boot**
- **Spring Security**
- **Auth0**
- **Lombok**
- **MySQL**
- **JPA**
- **Flyway**

## � Funcionalidades

### Autenticación y Autorización
- Implementación de seguridad stateless mediante JWT.
- Generación de tokens de autenticación para usuarios.

### CRUD de Autores
- **POST /autores:** Crear un nuevo autor.
- **GET /autores:** Obtener una lista de autores.
- **GET /autores/{id}:** Obtener un autor por ID.
- **PUT /autores:** Actualizar un autor (El ID va en el body del PUT).
- **DELETE /autores/{id}:** Eliminar un autor.

### CRUD de Tópicos
- **POST /topicos:** Crear un nuevo tópico.
- **GET /topicos:** Obtener una lista de tópicos.
- **GET /topicos/{id}:** Obtener un tópico por ID.
- **PUT /topicos/{id}:** Actualizar un tópico.
- **DELETE /topicos/{id}:** Eliminar un tópico.

## � Requisitos de Autenticación

Para todas las operaciones CRUD se requiere un token de autenticación, excepto para las siguientes:
- **POST /autores:** Registro de un nuevo autor.
- **POST /login:** Generación de un token de autenticación para un autor.

## � Próximas Actualizaciones

- **Implementación de Respuestas en los Tópicos:** Permitir a los usuarios responder a los tópicos.
- **Manejo de Permisos:** Asegurar que solo los usuarios puedan manipular sus propios tópicos y perfiles, evitando accesos no autorizados.

## � Endpoints

### Autores
- **POST /autores:** Crear un nuevo autor.
- **GET /autores:** Obtener una lista de autores.
- **GET /autores/{id}:** Obtener un autor por ID.
- **PUT /autores:** Actualizar un autor (El ID va en el body del PUT).
- **DELETE /autores/{id}:** Eliminar un autor.

### Tópicos
- **POST /topicos:** Crear un nuevo tópico.
- **GET /topicos:** Obtener una lista de tópicos.
- **GET /topicos/{id}:** Obtener un tópico por ID.
- **PUT /topicos/{id}:** Actualizar un tópico.
- **DELETE /topicos/{id}:** Eliminar un tópico.

### Autenticación
- **POST /login:** Generar un token de autenticación para un autor.

## � Cómo Empezar

### Prerequisitos
- Java 11 o superior.
- MySQL.
- Maven.

### Instalación

1. Clona el repositorio:
   ```sh
   git clone https://github.com/tuusuario/forohub.git

   2.Configura tu base de datos en application.properties:
   spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=tuusuario
spring.datasource.password=tucontraseña

Ejecuta la aplicación:
mvn spring-boot:run
� Contribuciones
¡Las contribuciones son bienvenidas! Si deseas contribuir, por favor haz un fork del proyecto y crea un pull request con tus cambios.

Desarrollado por kuromi04 durante la certificación en Alura Latam.

Puedes copiar este código y pegarlo directamente en tu archivo README.md. ¡Espero que te sea de ayuda!


