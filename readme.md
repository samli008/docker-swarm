## yum -y install ansible and cp hosts to /etc/ansible/
1. common.yaml
2. docker.yaml
3. keepalived.yaml
4. haproxy.yaml
5. load.yaml
6. docker swarm init --advertise-addr 192.168.6.131
7. docker swarm join-token manager
8. docker swarm join --token xxxxx 192.168.6.131
9. docker node ls
10. docker stack deploy -c nginx.yaml web
11. docker service ls
12. docker stack ls
