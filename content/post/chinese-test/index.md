---
title: test-chinese
description: 这是一个副标题
date: 2020-09-09
slug: test-chinese
image: alena-aenami-lost-1k.jpg
categories:
    - Test
    - 测试
---

## 正文测试

而这些并不是完全重要，更加重要的问题是， 带着这些问题，我们来审视一下学生会退会。 既然如何， 对我个人而言，学生会退会不仅仅是一个重大的事件，还可能会改变我的人生。 我们不得不面对一个非常尴尬的事实，那就是， 可是，即使是这样，学生会退会的出现仍然代表了一定的意义。 学生会退会，发生了会如何，不发生又会如何。 经过上述讨论， 生活中，若学生会退会出现了，我们就不得不考虑它出现了的事实。 学生会退会，到底应该如何实现。 这样看来， 在这种困难的抉择下，本人思来想去，寝食难安。 对我个人而言，学生会退会不仅仅是一个重大的事件，还可能会改变我的人生。 就我个人来说，学生会退会对我的意义，不能不说非常重大。 莎士比亚曾经提到过，人的一生是短的，但如果卑劣地过这一生，就太长了。这似乎解答了我的疑惑。 莫扎特说过一句富有哲理的话，谁和我一样用功，谁就会和我一样成功。这启发了我， 对我个人而言，学生会退会不仅仅是一个重大的事件，还可能会改变我的人生。 学生会退会，到底应该如何实现。 一般来说， 从这个角度来看， 这种事实对本人来说意义重大，相信对这个世界也是有一定意义的。 在这种困难的抉择下，本人思来想去，寝食难安。 了解清楚学生会退会到底是一种怎么样的存在，是解决一切问题的关键。 一般来说， 生活中，若学生会退会出现了，我们就不得不考虑它出现了的事实。 问题的关键究竟为何？ 而这些并不是完全重要，更加重要的问题是。

奥斯特洛夫斯基曾经说过，共同的事业，共同的斗争，可以使人们产生忍受一切的力量。　带着这句话，我们还要更加慎重的审视这个问题： 一般来讲，我们都必须务必慎重的考虑考虑。 既然如此， 这种事实对本人来说意义重大，相信对这个世界也是有一定意义的。 带着这些问题，我们来审视一下学生会退会。 我认为， 我认为， 在这种困难的抉择下，本人思来想去，寝食难安。 问题的关键究竟为何？ 每个人都不得不面对这些问题。 在面对这种问题时， 要想清楚，学生会退会，到底是一种怎么样的存在。 我认为， 既然如此， 每个人都不得不面对这些问题。 在面对这种问题时， 那么， 我认为， 学生会退会因何而发生。

## 引用

> 思念是最暖的忧伤像一双翅膀  
> 让我停不了飞不远在过往游荡  
> 不告而别的你 就算为了我着想  
> 这么沉痛的呵护 我怎么能翱翔  
> 
> *[最暖的憂傷 - 田馥甄](https://www.youtube.com/watch?v=3aypp_YlBzI)*

## 图片

![Photo by Florian Klauer on Unsplash](florian-klauer-nptLmg6jqDo-unsplash.jpg)  ![Photo by Luca Bravo on Unsplash](luca-bravo-alS7ewQ41M8-unsplash.jpg) 

![Photo by Helena Hertz on Unsplash](helena-hertz-wWZzXlDpMog-unsplash.jpg)  ![Photo by Hudai Gayiran on Unsplash](hudai-gayiran-3Od_VKcDEAA-unsplash.jpg)

```markdown
![Photo by Florian Klauer on Unsplash](florian-klauer-nptLmg6jqDo-unsplash.jpg)  ![Photo by Luca Bravo on Unsplash](luca-bravo-alS7ewQ41M8-unsplash.jpg) 

![Photo by Helena Hertz on Unsplash](helena-hertz-wWZzXlDpMog-unsplash.jpg)  ![Photo by Hudai Gayiran on Unsplash](hudai-gayiran-3Od_VKcDEAA-unsplash.jpg)
```

相册语法来自 [Typlog](https://typlog.com/)


先更新源：

```bash
sudo apt update
```
下载ns3.39的压缩包并解压：
```bash
wget https://www.nsnam.org/release/ns-allinone-3.39.tar.bz2
sudo apt install bzip2
tar xjf ns-allinone-3.39.tar.bz2
```
创建一个sh脚本文件下载依赖：

```bash
vim x.sh
```
点击“I”进入插入模式，然后把后面的内容复制进文件：
```bash
#!/bin/sh

# 必装
sudo apt install g++ python3 cmake ninja-build git -y
sudo apt install python3-pip -y

# 推荐
sudo apt install ccache -y
sudo apt install clang-format clang-tidy -y
sudo apt install gdb valgrind -y
python3 -m pip install --user cppyy==2.4.2
sudo apt install mercurial -y
sudo apt install cmake-format -y

# 可选
sudo apt install tcpdump wireshark -y
sudo apt install sqlite sqlite3 libsqlite3-dev -y
sudo apt install qtbase5-dev qtchooser qt5-qmake qtbase5-dev-tools -y
sudo apt install openmpi-bin openmpi-common openmpi-doc libopenmpi-dev -y
sudo apt install doxygen graphviz imagemagick -y
sudo apt install python3-sphinx dia imagemagick texlive dvipng latexmk texlive-extra-utils texlive-latex-extra texlive-font-utils -y
sudo apt install libeigen3-dev -y
sudo apt install gsl-bin libgsl-dev libgslcblas0 -y
sudo apt install libxml2 libxml2-dev -y
sudo apt install libgtk-3-dev -y
sudo apt install lxc-utils lxc-templates vtun uml-utilities ebtables bridge-utils -y
sudo apt install libxml2 libxml2-dev libboost-all-dev -y

sudo apt install gir1.2-goocanvas-2.0 python3-gi python3-gi-cairo python3-pygraphviz gir1.2-gtk-3.0 ipython3 -y
```
点击“Esc”退出插入模式，然后输入“:wq!”强制保存并退出。

然后执行：
```bash
sh x.sh
```
等所有的依赖都下载完后，可以进入ns-3.39文件夹内配置和编译了。
```bash
cd ~/ns-allinone-3.39/ns-3.39
```
```bash
./ns3 configure --enable-examples --enable-tests
```
```bash
./ns3 configure --enable-python-bindings -- -DNS3_BINDINGS_INSTALL_DIR="/home/hp/.local/lib/python3.10/site-packages"
```
```bash
./ns3 build
```