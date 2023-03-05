
# 前言

&emsp; 个人在使用python和运行vs还有git的时候，感觉还是经常会用到cmd相关的命令，而课堂上只是学习过linux相关的命令，和cmd又有些不同，经常会出错，故此总结记录一下，以后也方便自己进行查找翻看。
适合与Linux命令结合学习，注意异同点[[Linux]]

# 0. 启动

<kbd>Win</kbd> + <kbd>r</kbd> 进入运行，输入cmd
按下<kbd>Enter</kbd>进入cmd；
按下<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>Enter</kbd>使用管理员权限启动



# 1. 常用命令

## 1.1 跳转硬盘
```
d:   //跳转到D盘
f:   //跳转到F盘

cd /d d: //加参数/d跳转到D盘
```
## 1.2 cd命令
```
cd /?    //获取使用帮助
cd \    //根目录

cd ..     //上级目录               
cd test    //进入当前目录下的test文件夹
cd c:\test1  //跳转当前磁盘下的其他文件夹
```
## 1.3 查看文件目录
```
dir //查看当前文件夹下的文件

//该命令类似于linux的ls命令，经常混淆

dir /?   //查看隐藏文件夹
```

### 1.4 清除屏幕
```
cls //类似Linux的clear
```
### 1.5 查看ip与网络相关
```
ipconfig  //查看ip

ping [ip] //测试与【ip】的连接是否畅通

netstat -ano //查看网络连接、状态与对应进程id
```
### 1.6 创建删除文件夹（目录）
```
md Dir1 //创建文件夹Dir1
rd Dir1 //删除文件夹Dir1
```
### 1.7 删除复制移动文件
```
copy [文件path1] [文件path2] //把文件从一个位置复制到另一个位置

move [文件path1] [文件path2] //把文件从一个位置移动到另一个位置

del File1 //删除文件File1，仅能删除文件，不能删除文件夹

```

### 查看帮助
```
-help
/?
```

# 2. Git命令的相关使用

# 3. Python相关使用

下载python的库命令pip [[Pip——Python的包管理工具]]

# 4. Visual Studio的相关使用

# 5. Java相关使用