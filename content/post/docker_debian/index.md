---
title: 在debian12上安装docker
description: 在Ubuntu上
date: 2025-01-13
slug: docker_debian
image: alena-aenami-lost-1k.jpg
categories:
    - debian
---

```bash
sudo apt-get remove docker docker-engine docker.io
sudo apt-get install apt-transport-https ca-certificates curl gnupg2 software-properties-common
```


```bash
curl -fsSL https://mirrors.huaweicloud.com/docker-ce/linux/debian/gpg | sudo apt-key add -
```


```bash
sudo add-apt-repository "deb [arch=amd64] https://mirrors.huaweicloud.com/docker-ce/linux/debian $(lsb_release -cs) stable"
```


```bash
sudo apt-get update
sudo apt-get install docker-ce
```

```bash
sudo groupadd docker
sudo usermod -aG docker $USER
sudo systemctl restart docker
sudo chmod o+rw /var/run/docker.sock
```

```bash
docker ps -a
```
