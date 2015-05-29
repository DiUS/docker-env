commands
--------
```shell
$ docker run -i -t --rm ubuntu:14.04 /bin/bash
```
* inside
```shell
$ ls -la
$ top
$ foo
$ dpkg -l
$ netstat -lnpt
$ uname -r
```

```shell
docker run -i -t --name first_guest ubuntu:14.04 /bin/bash
```

```shell
docker ps
```

```shell
docker images
```

```shell
docker ps -a
```

```shell
docker build -t scheffield/first-image .
```

```shell
docker build -t scheffield/custcollection:v1.0 .
```

```shell
docker run -i -t --rm -p 8080:8080 scheffield/custcollection:v1.0
```

```shell
docker create --name custcollection -p 8080:8080 scheffield/custcollection:v1.0
```

```shell
docker start custcollection
```

```shell
docker stop custcollection
```
