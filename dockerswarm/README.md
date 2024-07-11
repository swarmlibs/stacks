# About

TBD

## Install

First, retrieve the stack YML manifest:
```sh
curl -L https://raw.githubusercontent.com/swarmlibs/stacks/main/dockerswarm/docker-stack.yml -o dockerswarm-stack.yml
```

Then use the downloaded YML manifest to deploy your stack:
```sh
docker stack deploy -c dockerswarm-stack.yml dockerswarm
```

## One-line installer

```sh
curl -L https://raw.githubusercontent.com/swarmlibs/stacks/main/dockerswarm/docker-stack.yml | docker stack deploy -c - dockerswarm
```

Docker Swarm Stack have now been installed. You can check to see whether the all services have started by running `docker service ls`:
```sh
root@manager01:~# docker service ls
ID             NAME                        MODE         REPLICAS               IMAGE                                 PORTS
lutfgiv4xtcx   dockerswarm_node_metadata   replicated   1/1 (max 1 per node)   swarmlibs/node-metadata-agent:local
```
