# Linuxowy kontener z openjdk v17
FROM openjdk:17-jdk-slim

# Ustawianie katalogu roboczego w kontenerze
WORKDIR /app

# Skopiowanie pliku JAR z hosta do kontenera
COPY target/rest-service-0.0.1-SNAPSHOT.jar /app/rest-service.jar

# Wystawienie portu 8080 (domyślny port dla aplikacji Spring Boot)
EXPOSE 8080

# Uruchomienie aplikacji spring-bootowej przy starcie kontenera
ENTRYPOINT ["java", "-jar", "/app/rest-service.jar"]
