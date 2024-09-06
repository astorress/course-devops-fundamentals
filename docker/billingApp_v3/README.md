# Tecnical details of programas
    1- The .JAR billing-0.0.3-SNAPSHOT.jar listening or port 8080
    2- The .JAR billing-0.0.2-SNAPSHOT.jar listening or port 7080
    3- You should keep the same port (internal an external) for backend port mapping in order to avoid mistakes with angular app.
    4- The angular app are point to the fix socket http://localhost:7080 for back prep y http://localhost:8080 for back prod
    5- The volume data for postgres should be different for producction and preproduction

