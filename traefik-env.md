```sh
docker network create --driver overlay --attachable webproxy
```

```sh 
export NODE_ID=$(docker info -f '{{.Swarm.NodeID}}')
docker node update --label-add traefik-public.traefik-public-certificates=true $NODE_ID
```

```sh 
export USERNAME=admin
export HASHED_PASSWORD=$(openssl passwd -apr1)
echo $HASHED_PASSWORD
export DOMAIN=traefik.13.ipv9.xyz
```
