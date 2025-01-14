---
title: hugo + github.io
description: 在Ubuntu上
date: 2025-01-13
slug: hugo
image: alena-aenami-lost-1k.jpg
categories:
    - hugo
    - Ubuntu
---

先create repository

只需要填上`Repository name`那一栏，格式为`<name>.github.io`。如果你想让你的博客网址就是`.github.io`，则`<name>`不能是任意名字，必须是你的github用户名。

确保`Add a README file`勾上，然后点击`Create repository`就行了。

点绿色的`Code`，点`Codespaces`，点`Create Codespaces on main`
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```
echo >> /home/codespace/.bashrc
echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> /home/codespace/.bashrc
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```

```
brew install hugo
```
```
cd ..
hugo new site cetcsc.github.io --force
cd cetcsc.github.io
```
```
git init
git submodule add https://github.com/CaiJimmy/hugo-theme-stack/ themes/hugo-theme-stack
cp -r themes/hugo-theme-stack/exampleSite/* /workspaces/cetcsc.github.io
rm hugo.toml
```
然后在左侧的“源代码管理”中，随便填一段话，点“提交并推送“。

下一步是进入`https://github.com/<name>/<name>.github.io`，点击上方栏的`Settings`，然后点击左方栏的`Pages`，在`Build and deployment`里的`Source`中选择`Github Actions`，在下面找到`Hugo`，点击`Configure`，在新界面点击右侧的绿色按钮的`Commit changes...`。

找不到`Hugo`就去`browse all workflows`里找。

然后hugo就开始在github上部署了，部署好后就可以在`Pages`页面看到`Your site is live at ...`，点击`Visit site`就可以访问博客网站了。

后续只需在相应的文件夹下添加.md文件再点“提交并推送“，就可以更新博客了





