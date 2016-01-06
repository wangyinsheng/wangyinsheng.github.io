---
layout: page
title: Install Lua!
tagline: Supporting tagline
---
{% include JB/setup %}

##安装Lua

###下载Lua源码
        wget http://www.lua.org/ftp/lua-5.3.2.tar.gz

###下载libreadline的相关包，否则编译时提示找不到readline.h
        sudo apt-get install libreadline5
        sudo apt-get install libreadline-dev

###编译源码
        tar xzf lua-5.3.2.tar.gz
        cd lua-5.3.2
        make linux
        sudo make install

###测试
        silver@ubuntu:~$ lua
        Lua 5.3.2  Copyright (C) 1994-2015 Lua.org, PUC-Rio
        >


