# docker-bash-example

A simple docker example that provides a debian linux os with node 14 installed.

This example image is available on dockerhub: https://hub.docker.com/repository/docker/wwlib/docker-examples

### build
To build the example Dockerfile locally:
```
docker build -f Dockerfile -t wwlib/docker-examples:bash "."
```

### run
```
docker run -it wwlib/docker-examples:bash
```

This will start a bash prompt, like:

```
root@f56f6421a21e:/usr/src/app#
```

Try it out using:
```
# cat /etc/issue
Debian GNU/Linux 9 \n \l

# cat /etc/os-release
PRETTY_NAME="Debian GNU/Linux 9 (stretch)"
NAME="Debian GNU/Linux"
VERSION_ID="9"
VERSION="9 (stretch)"
VERSION_CODENAME=stretch
ID=debian
HOME_URL="https://www.debian.org/"
SUPPORT_URL="https://www.debian.org/support"
BUG_REPORT_URL="https://bugs.debian.org/"

# node --version
v14.18.2

# git version
git version 2.11.0

# pwd
/usr/src/app

# ls -al
total 16
drwxr-xr-x 1 root root 4096 Jan 11 22:25 .
drwxr-xr-x 1 root root 4096 Jan 11 22:25 ..
-rw-r--r-- 1 root root   30 Jan 11 22:11 index.js

# node index.js
Hello, world!
```

Now you have a Debian linux shell.

To exit:
```
# exit
```
