---
title: "如何用hugo搭建个人博客"
date: 2019-08-20T11:50:45+08:00
draft: false
---

### 1.进入 hugo 官网，点击 Quick Start 进入。按照步骤去做。
### 2.安装 hugo。 
    windows安装

* 进入 Hugo Releases 页面，点击 Assets,下载 hugo_XXX_Windows-64bit.zip。
* 解压至某个文件夹，将复制相应路径加至 PATH。
  加至PATH的方法为：
  
  * 右键点击 <此电脑>
 
  * 找到 属性 -> 高级系统设置 -> 环境变量-> path
 
  * 复制路径加至 PATH
  
  * 启动终端，运行
  ```
    hugo version
  ``` 
  * 看到版本号，则表明安装成功了。

### 3.安照 Step2-Step7 ，复制代码，然后在终端运行。
* 其中 Step2，在 D盘 创建新文件夹 xxx，在其运行在
  ```
  hugo new site username.github.io-creator 
  ```
  在 xxx 创建 username.github.io-creator 文件夹，在此文件夹中运行之后步骤。
* 其中 Step6 ,在 VsCode 里用 Ctrl+Shift+P 快捷键打开 config.toml。
  * 汉化，将 Language,从 en 改成 zh-Hans,title 也可以改成自己喜欢的名字。
* 新开一个终端运行 hugo。 
### 4.最后，运行 Step7:hugo 之后，出现 public 文件，我们需要将 public 文件提交至 github 上。
 
* 回到终端，新建 .gitignore,在其写
  ```
  /public/
  ```  
* 复制SSH地址。
  ```
  cd public
  git init
  git add .
  git commit -v
  ```
* 此时在 github 上新建仓库 username.github.io (username为你的用户名)。复制SSH地址。
```
     git@github.com......
     git push -u origin master
```
* 进入 github -> username.github.io ->settings,找到 Github Pages，在 source 上方的选项，选中 master 分支。
* 点击绿色框的地址就可以看见自己的博客啦。

  