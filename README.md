<h1 align="center">Ganache Docker Example</h1>
<p align="center">Ganache local chain with fixed private key Dockerfile and docker-compose example</p>
<div align="center">

</div>

## Getting Started

```
git clone https://github.com/ft-jasong/ganache-docker-example.git
cd ganache-docker-example
```

### Start with Dockerfile

```
docker build --build-arg \
NODE_VERSION=<NODE_VERSION> \
GANACHE_VERSION=<GANACHE_VERSION> \
PRIV_KEY=<PRIVATE_KEY> \
INIT_WEI=<INIT_WEI> \
-t <IMAGE_NAME:TAG> .
```

and run this command

```
docker run -d -p <PORT>:8545 <IMAGE_NAME:TAG>
```

### Start with docker-compose

Set your settings args section in docker-compose.yml and run the command

```
docker-compose up -d
```
