# Docker Super Mario

## ❌ No docker-desktop on my Archlinux !

## Pull the image
```bash
docker pull pengbai/docker-supermario:latest

```

## Show/List Image
```bash
docker images | grep mario

```

##  Run image in container with port 8600:8080
```bash
docker run -d -p 8600:8080 --name supermario pengbai/docker-supermario

```
![Run](images/Screenshot_25-juil._14-53-22_5390.png)


##  Open SuperMario

```bash
localhost:8600
```

![AccessLocalhost](images/Screenshot_25-juil._15-04-55_28226.png)


##  Stop & Remove container 
```bash
docker rm -f supermario
```
OR
```bash
docker stop supermario && docker rm supermario
```


##  Remove Image

```bash
docker rmi pengbai/docker-supermario

```

![Clean](images/Screenshot_25-juil._15-09-21_17678.png)

