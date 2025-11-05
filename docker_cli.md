## List all containers running

```shell
docker ps
```

## List all containers including stopped containers

```shell
docker ps -a
```

## To run 

```shell
docker run nginx
```

## To run in detached mode

```shell
docker run -d nginx
```

## To run in detached mode and expose a port and name the  container

```shell
docker run --name web_server -d -p 8080: 80 nginx
```

## To stop container

```shell
docker stop < container name >
```

## To remove container

```shell
docker rm < container ID >
```

## To filter containers


```shell
docker docker ps | grep web_server
```

(or the preferred way) 

```shell
docker docker ps --filter name=web_server
```

## Remove multiple containers 

```shell
docker docker rm  $(docker ps -aq)
```