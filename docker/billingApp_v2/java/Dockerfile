# Usa una imagen base con JRE 17 en Alpine
FROM eclipse-temurin:17-alpine

# Create a new group with specific uid and non-root user called "admin"
# Be sure that group id are not present on host. if already exist change by arbitrary other uid
RUN addgroup -g 1028 devopsc \
    && adduser -D -G devopsc admin

# Create a new mount point at /tmp on native host because a volume is more efficient and faster than filesystem
VOLUME /tmp

# Copiamos el jar a la imagen
ARG JAR_FILE

# Establece una variable de entorno para la contraseña de la base de datos
ARG DB_PASSWORD

# Establece la variable de entorno DB_PASSWORD con el valor del argumento
ENV DB_PASSWORD=qwerty

# Copia el archivo JAR
COPY ${JAR_FILE} /tmp/app.jar

# Change ownership of the /app directory to the "admin" user
RUN chown -R admin:devopsc /tmp

# Cambia al usuario 'admin'
USER admin

# Ejecutamos el jar al iniciar el contenedor
ENTRYPOINT ["java","-jar","/tmp/app.jar"]
