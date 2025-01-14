---
title: debian12的国内镜像源
description: 在Ubuntu上
date: 2025-01-13
slug: mirror_debian
image: alena-aenami-lost-1k.jpg
categories:
    - debian
---

```bash
/etc/apt/sources.list
```

阿里云

```bash
deb https://mirrors.aliyun.com/debian/ bookworm main non-free non-free-firmware contrib
deb-src https://mirrors.aliyun.com/debian/ bookworm main non-free non-free-firmware contrib
deb https://mirrors.aliyun.com/debian-security/ bookworm-security main
deb-src https://mirrors.aliyun.com/debian-security/ bookworm-security main
deb https://mirrors.aliyun.com/debian/ bookworm-updates main non-free non-free-firmware contrib
deb-src https://mirrors.aliyun.com/debian/ bookworm-updates main non-free non-free-firmware contrib
deb https://mirrors.aliyun.com/debian/ bookworm-backports main non-free non-free-firmware contrib
deb-src https://mirrors.aliyun.com/debian/ bookworm-backports main non-free non-free-firmware contrib
```

兰州大学

```bash
deb https://mirrors.lzu.edu.cn/debian/ bookworm main non-free non-free-firmware contrib
deb-src https://mirrors.lzu.edu.cn/debian/ bookworm main non-free non-free-firmware contrib
deb https://mirrors.lzu.edu.cn/debian-security/ bookworm-security main
deb-src https://mirrors.lzu.edu.cn/debian-security/ bookworm-security main
deb https://mirrors.lzu.edu.cn/debian/ bookworm-updates main non-free non-free-firmware contrib
deb-src https://mirrors.lzu.edu.cn/debian/ bookworm-updates main non-free non-free-firmware contrib
deb https://mirrors.lzu.edu.cn/debian/ bookworm-backports main non-free non-free-firmware contrib
deb-src https://mirrors.lzu.edu.cn/debian/ bookworm-backports main non-free non-free-firmware contrib
```

华为云

```bash
deb https://mirrors.huaweicloud.com/debian/ bookworm main non-free non-free-firmware contrib
deb-src https://mirrors.huaweicloud.com/debian/ bookworm main non-free non-free-firmware contrib
deb https://mirrors.huaweicloud.com/debian-security/ bookworm-security main
deb-src https://mirrors.huaweicloud.com/debian-security/ bookworm-security main
deb https://mirrors.huaweicloud.com/debian/ bookworm-updates main non-free non-free-firmware contrib
deb-src https://mirrors.huaweicloud.com/debian/ bookworm-updates main non-free non-free-firmware contrib
deb https://mirrors.huaweicloud.com/debian/ bookworm-backports main non-free non-free-firmware contrib
deb-src https://mirrors.huaweicloud.com/debian/ bookworm-backports main non-free non-free-firmware contrib
```