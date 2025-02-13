## SETUP DOCKER ELK STACK 

pertama clone git, lakukan di direktori mana saja

kedua jika sudah lakukan setup
```
docker compose up setup
```

jika sudah setup, running container
```
docker compose up
```

config sudah beres.

jika ingin melakukan config, lakukan pada file
```
logstash.conf, logstash_writer.json, docker-compose.yml
```

jika ingin mengubah password untuk ELK (elasticsearch, logstash, kibana) pada file .env,
jika sudah lakukan reset dengan command
```
docker compose exec elasticsearch bin/elasticsearch-reset-password --batch --user elastic
```
```
docker compose exec elasticsearch bin/elasticsearch-reset-password --batch --user logstash_internal
```
```
docker compose exec elasticsearch bin/elasticsearch-reset-password --batch --user kibana_system
```
