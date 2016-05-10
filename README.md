# docker-wp-nginx

forked from https://github.com/eugeneware/docker-wordpress-nginx.git

```bash
$ git clone https://github.com/l9c/docker-wp-nginx.git
$ cd docker-wp-nginx
$ sudo docker build -t="l9c/docker-wp-nginx" .
```

## Usage

To spawn a new instance of wordpress on port 80.  The -p 80:80 maps the internal docker port 80 to the outside port 80 of the host machine.

```bash
$ sudo docker run -p 80:80 --name docker-wp-nginx -d l9c/docker-wp-nginx
```

Start your newly created docker.

```
$ sudo docker start docker-wp-nginx
```

After starting the docker-wordpress-nginx check to see if it started and the port mapping is correct.  This will also report the port mapping between the docker container and the host machine.

```
$ sudo docker ps

0.0.0.0:80 -> 80/tcp docker-wp-nginx
```

You can the visit the following URL in a browser on your host machine to get started:

```
http://127.0.0.1:80
```
Shell operation
```
docker exec -it xxxxxxxx /bin/bash 
docker exec -it <container_name> /bin/bash
```
