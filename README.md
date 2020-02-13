Docker-PHPs
====

Build php container 7.3.14, 5.6.4 and 5.1.6

## Install

```bash
$ docker-compose up -d
$ docker exec -it php-5.1.6 bash
$ docker exec -it php-5.6.4 bash
$ docker exec -it php-7.3.14 bash
```

## Web Access

```bash
# php-7.3.14
$ open http://localhost:4001

# php-5.6.4
$ open http://localhost:4002

# php-5.1.6
$ open http://localhost:4003
```
