# docker-sample-nginx

a sample nginx container to display container name


Build Image

```bash
$ docker build -t my-nginx .
```

Start a container

```bash
$ docker run -d --rm --name container-name-what-you-want -p 8080:80  my-nginx 
```

Check running container instance

```bash
$ docker ps 
```

Connect to the container
```bash
$ docker exec -it container-name-what-you-want /bin/sh 
```

Stop container

```bash
$ docker stop container-name-what-you-want
```
