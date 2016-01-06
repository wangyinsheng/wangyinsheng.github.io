---
layout: page
title: Hello World!
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


Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)

## Update Author Attributes

In `_config.yml` remember to specify your own data:
    
    title : My Blog =)
    
    author :
      name : Name Lastname
      email : blah@email.test
      github : username
      twitter : username

The theme should reference these variables whenever needed.
    
## Sample Posts

This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

    $ rm -rf _posts/core-samples

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

This theme is still unfinished. If you'd like to be added as a contributor, [please fork](http://github.com/dbtek/jekyll-bootstrap-3)!


