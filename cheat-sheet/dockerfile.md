---
title: Dockerfile Cheat Sheet
author: Danny Cheung
tags:
  - docker
  - dockerfile
  - cheat sheet
---

| Command | Description |
| ------- | ----------- |
| ```FROM <image_name>``` | Specify the image to use. <br> !! MUST be the first instruction !! |
| ```FROM <image_name>:<tag>``` | Specify the image (and version) to use. <br> !! MUST be the first instruction !! |
| ```FROM <image_name>@<digest>``` | Specify the image (and version) to use. <br> !! MUST be the first iinstruction !! |
| ```MAINTAINER <author_name>``` | Specify an author |
| ```ENV <variable_name>=<value>``` | Specify an evnironment variable called <var>variable_name</var> |
| ```RUN <command> [<parameter> ...]``` | Inside the container, execute <var>command</var> inside a shell as part of the setup |
| ```RUN ["<executable>", "<parameter>",...]``` | Inside the container, execute <var>executable</var> with the parameters as part of the setup. <br> !! Must use double-quotes !! <br> !! Not run inside shell !! |
| ```CMD <command> [<parameter> ...]``` | Service/Process that container is designed to provide. |
| ```CMD ["<command>", ["<parameter>",...]``` | Service/Process that container is designed to provide. <br> !! Must use double-quotes !! <br> !! Not run inside shell !! |
| ```LABEL <label_key>=<label_value> ...``` | Specify a label for the container. |
| ```EXPOSE <port> [<port> ...] ``` | Specify port(s) that container will listen on. <br> !! Need to use links to connect container ports to host ports |
| ```ADD <src> <dest>``` | Copy files from <var>src</var> to <var>dest</var> <br> <src> can be a remote URL |
| ```VOLUME <mount_point> ...``` | Specify mount points |
| ```USER <user>``` | User when executing RUN and CMD |
| ```${variable_name}``` | Use a variable inside the Dockerfile |
