* Projekt `demo` loguje standardnim Spring Boot zpusobem

cd demo

# Provede build image aplikace
mvnw spring-boot:build-image

cd ..

# Spusti elasticsearch, kibana, fluentd & aplikaci
docker-compose up --build

# Poznamka ke zpusobu logovani:

Pouziva se fluentd logging driver z Dockeru

# Kibana:
http://localhost:5601

# Vsechno smazne:
docker-compose down
