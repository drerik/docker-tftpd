# Docker tftp container

## Build
You can build the docker container localy using this command:

```
docker build -t drerik/tftpd https://github.com/drerik/docker-tftpd.git
```

## Run
To start a tftp container with the current dir as share like this:
 
```
docker run -it --rm -p 69:69 -v $(pwd):/var/lib/tftpboot --name tftpd drerik/tftpd
```