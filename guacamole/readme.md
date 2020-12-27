## docker swarm deploy guacamole
1. load_mole.yaml
2. ansible node -a 'mkdir /mysql'
3. ansible node -a 'mount k4:/data/mysql /mysql'
4. docker stack deply -c guacamole.yaml mole
5. docker service ps mole_mysql
6. docker cp initdb.sql ***containerID***:/root/
7. docker exec -it ***containerID*** /bin/bash
8. mysql -u root -pliyang guacamole_db < /root/initdb.sql
