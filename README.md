<h1 align="center">Fixed Key Ganache Example</h1>
<p align="center">Ganache local chain Dockerfile and docker-compose example set with fixed private key</p>
<div align="center">

</div>

## Getting Started

```
git clone https://github.com/ft-jasong/fix-key-ganache-docker.git
cd fix-key-ganache-docker
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
