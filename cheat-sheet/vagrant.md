---
title: Vagrant Cheat Sheet
author: Danny Cheung
tags:
  - vagrant
  - cheat sheet
---

| Command | Description |
| ------- | ----------- |
| ```vagrant up``` | Build the environment as specified by ./Vagrantfile |
| ```vagrant ssh [<hostname>]``` | SSH into a host. If there is only one host specified in .\Vagrantfile, the hostname is optional  |
| ```vagrant destroy [-f] [<hostname>]``` | Destroy a host. If no host is specified, all hosts will be destroyed. Use to -f to disable prompt.  |
