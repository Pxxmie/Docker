## Setting up Docker

### Running Nginx in a Docker Container

```bash
$ docker run -d -p 80:80 nginx
68206eeac64ba31df5225ba3da46790ae089f2f8f77f9c248dcc293fc32d9b99

Prismika@Pris MINGW64 ~/Desktop
$ docker ps
CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS          PORTS                NAMES
68206eeac64b   nginx     "/docker-entrypoint.…"   13 seconds ago   Up 13 seconds   0.0.0.0:80->80/tcp   friendly_elgamal
```

![Alt text](images/nginx.png)

### Access Nginx from local host

Open your web browser and navigate to http://localhost. You should see the 
default Nginx welcome page.

![Alt text](<images/Screenshot 2023-10-30 132620.png>)

### Stop and Start the Container 


```
docker ps 
```

![Alt text](images/dockerps.png)


```
docker stop <CONTAINERID>

docker start <CONTAINERID>
```
![Alt text](images/dockerstart_stop.png)

### Remove the container

```
docker rm <CONTAINERID> -f
```
![Alt text](images/DOCKERRM.png)

### Access the Shell inside the Docker container


```bash
docker exec -it 97b47349673e sh
```

![Alt text](images/access_dockercontainer.png)

Install Dependencies: 

```
apt update 

apt upgrade -y 

apt install sudo

apt install nano
```
