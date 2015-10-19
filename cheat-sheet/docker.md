---
title: Docker Cheat Sheet
author: Danny Cheung
tags:
  - docker
  - cheat sheet
---

| Command | Description |
| ------- | ----------- |
| ```docker ps``` | List running containers |
| ```docker images``` | List locally available images |
| ```docker run``` <br> ```[--name <container_name>]``` <br> ```[-v <host_dir>:<mount_point>]``` <br> ```[-P | -p <host_port>:<container_port>]``` <br> ```<image_name> <command>``` | Run a command in a new container based on an image |
| ```docker create <image_name> --name=<container_name>``` | Create a container of name <var>container_name</var> and is based off <var>image_name</var> |
| ```docker pull <image_name>``` | Retrieve an image from to the repo to local |
