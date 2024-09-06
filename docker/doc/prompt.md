# Props for chatGPT
- **Create a Spring boot maven Docker Image**
Creame una imagen de docker para un microservicio de spring boot 3 con maven y el jre 17, 
quiero que la imagen implemente la técnica de usuario rootless y que el jar como parámetro al momento de ejecutar el docker build

- **Create a JRE docker Image**
  - **1. Part**
Creame una imagen de docker para un microservicio de spring boot 3 que tenga como imagen base un jre 17 alpine,
 quiero que la imagen implemente la tecnica de usuario rootless, que agrege un grupo llamado devopsc y un usuario admin 
 que pertenezca a dicho grupo y que acepte el jar  como parametro al momento de ejecutar el docker build.
 
  - **2 Part**
 Redefine la imagen para agregar un argumento llamado DB_PASSWORD.

   - **3 Part**
 Agrega una varaible de entorno llamada DB_PASSWORD e inicializala con el argumento previamente definido.

- **Create a Postgres docker compose orchestration**
Creame una orquestacion de docker compose para una base de datos postgres con un administrador adminer, agrega un volumen para los datos de postgres y un volumen que monte un script de inicialización de la base de datos 