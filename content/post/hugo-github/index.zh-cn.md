---
title: hugo github
description: hugo github
date: 2023-07-09
slug: hugo github
image: helena-hertz-wWZzXlDpMog-unsplash.jpg
categories:
    - hugo
    - github
---


# 前置

## hugo下载

```
choco install hugo-extended
```

# 本地创建网站

## hugo new site <名字>

```
hugo new site
```

```
cd 
```

```
git init
```

## git submodule add <主题地址> themes/<主题名称>

```
git submodule add
```

把hugo.toml文件名改成config.toml

在config.toml文件里加上theme = '<主题名称>'

```
theme = '<主题名称>'
```

把baseURL 项改成 'https://<仓库名>.github.io/'

```
baseURL =  'https://<仓库名>.github.io/'
```



```
hugo server
```



git remote add origin <仓库路径>

```
git remote add origin 
```



```
git add .
```



```bash
git commit -m "first commit"
```



```bash
git push -u origin master
```