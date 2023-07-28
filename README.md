# mindbend2023 Project

Steps:-
1) Login to AWS account
2) Click on Master-swarm instances and connect it through EC2 instance connect.
3) Do same with other 2 swarm-worker instances(Used for container replications in Swarm).

Comands:
- docker stack deploy -c docker-compose.yaml mindbend  (It will deploy the web on public_IP:2377 of Master-Swarm)
- docker node ls                                       (To check the Swarm Manager and worker nodes)
- docker service ls                                    (To check initiated services on docker swarm)
- docker service rm <service_name>                      (To stop the service)
