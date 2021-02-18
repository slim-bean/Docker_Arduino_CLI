## Arduino-CLI Version

![Latest Version released by Arduino:](https://img.shields.io/github/release/arduino/arduino-cli.svg) 

Uses the latest Arduino-CLI image 0.16.0 ![Adafruit Library for releases](https://img.shields.io/github/v/release/arduino/arduino-cli.svg)

## Using the image

The image is available on [docker hub](https://hub.docker.com/repository/docker/jpconstantineau/arduino-cli/general). 

To use the docker image, do a docker pull, then you can call the CLI as part of the docker run command.

Note that to see your sketch, the working directory must be mounted in the image.

```
docker pull jpconstantineau/arduino-cli

docker run -it --mount src=${PWD},target=/mnt,type=bind  jpconstantineau/arduino-cli:latest arduino-cli

```


## Building the image yourself

```

 docker build .

```
