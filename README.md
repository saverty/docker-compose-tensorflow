# docker-compose-tensorflow

## Abstract

This project provides example configurations of docker compose for TensorFlow.

* docker-compose.yml

  * Single container

* distributed.yml

  * One parameter server and two worker

This project also provides Dockerfile referenced from the above docker compose configuration.
You can install Keras by using this Dockerfile.

## Using nvidia-docker-compose

You can use https://github.com/eywalker/nvidia-docker-compose to use GPUs in these examples.

e.g.

```
$ nvidia-docker-compose -f distributed.yml up -d
```

The GPU devices are specified in distributed.yml as an example.
You can change the configuration about devices.