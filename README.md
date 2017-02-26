# Docker container for the PoS course

## Requirements

Docker, [Docker compose](https://github.com/docker/compose/releases) (easy to install)

## Running 

To run the container and attach a shell to it, just run

```
./start
```

It will:
- rebuild the image from the Dockerfile if necessary
- run the container
- cleanup the container once you exit the shell

If for some reason you just want to rebuild (if necessary) and run the container in the background, use

```
cd container
docker-compose up -d --build
```

You can later run a shell in it by running

```
docker exec -it progos bash
```
