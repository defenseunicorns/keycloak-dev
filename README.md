delete the keycloak cluster

```
k3d cluster delete keycloak-dev
```

create the keycloak k3d cluster
```
k3d cluster create keycloak-dev --k3s-arg '--debug@server:0' -p '443:443@loadbalancer' -p '80:80@loadbalancer'   --k3s-arg='--disable=traefik@server:0'
```
