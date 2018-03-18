1. `docker swarm init`
	* or `docker swarm init --advertise-addr $(docker-machine ip node-1)
` 
2. `docker stack deploy -c ./stack.yml infinite-swarm`