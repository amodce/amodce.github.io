---
title: test-chinese copy
description: 这是一个副标题
date: 2023-08-08
slug: test-chinese copy
image: alena-aenami-lost-1k.jpg
categories:
    - Test
    - 测试
---


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