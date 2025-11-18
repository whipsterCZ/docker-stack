# RabbitMQ in docker-compose

## Setup
This setup assumes you already have docker-compose and docker (using docker toolbox) installed.

```
docker-compose up
```

## Play
Open [http://localhost:15672/](http://localhost:15672/) (or what ever IP you get when you run `docker-machine ip`)
Open [http://rabbitmq.loc/](http://rabbitmq.loc/) 
```
open http://$(docker-machine ip default):15672/
```
and use the login

```
username: admin
password: rabbitmq
```

## License
MIT License
