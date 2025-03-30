# Sprawozdanie z Laboratorium 5

# 1. Budowanie obrazu
```shell
docker build -f Dockerfile --build-arg VERSION=1.0.1 -t webapp .
```
![docker build](img/docker_build.png)

# 2. Uruchomienie kontenera
```shell
docker run -d -p 8080:80 --name app webapp
```
![docker run](img/docker_run.png)

# 3. Potwierdzenie działania kontenera
```shell
docker ps
```
![docker ps](img/docker_ps.png)

# 4. Potwierdzenie działania serwera
```shell
curl localhost:8080
```
![curl](img/docker_curl.png)
![browser](img/browser.png)


