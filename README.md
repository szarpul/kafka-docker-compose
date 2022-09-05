* ### RUN DOCKER COMPOSE FILE
> docker-compose up

* ### CREATE TOPIC
> docker exec kafka_1 kafka-topics --bootstrap-server kafka-2:9092 --create --topic first_topic

* ### OR CONNECT TO DOCKER CONTAINER AND CREATE A TOPIC
> docker container exec --it kafka_1 bash
> kafka-topics --bootstrap-server localhost-2:9092 --create --topic first_topic

* ### CLEAN UP
> docker-compose rm