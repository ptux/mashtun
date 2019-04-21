# volume bind mount insight

observe behavior of volume and bind mount on Docker For Mac

```shell
$ docker version
Client: Docker Engine - Community
 Version:           18.09.1
 API version:       1.39
 Go version:        go1.10.6
 Git commit:        4c52b90
 Built:             Wed Jan  9 19:33:12 2019
 OS/Arch:           darwin/amd64
 Experimental:      false

Server: Docker Engine - Community
 Engine:
  Version:          18.09.1
  API version:      1.39 (minimum version 1.12)
  Go version:       go1.10.6
  Git commit:       4c52b90
  Built:            Wed Jan  9 19:41:49 2019
  OS/Arch:          linux/amd64
  Experimental:     false
```

## create lab

```shell
### tty0
$ mkdir vol-insight
$ cd vol-insight
$ bash -c 'docker run -it --name vol-insight -v /vol -v $(pwd)/dir1:/dir2 busybox /bin/sh'
/ # ls
bin   dev   dir2  etc   home  proc  root  sys   tmp   usr   var   vol
```

```shell
### tty1
$ cd vol-insight
$ ls
dir1
$ docker volume ls
DRIVER              VOLUME NAME
local               92f1f1077cc5419e93bdef74994dd119e0a00dad710a5b4925cb87032945819c
```

```shell
### tty3
$ screen ~/Library/Containers/com.docker.docker/Data/com.docker.driver.amd64-linux/tty
[enter]
linuxkit-025000000001:#
```

## observe behavior

to be continued
...