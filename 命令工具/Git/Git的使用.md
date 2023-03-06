# 0. 简单认识Git
## 0.1 起源
  最初是由linux开发者linus用两周时间用c语言编写而成。github就是使用git系统对网站进行管理，github只支持git分布式系统，故名为github。

## 0.2 分布式
  svn和cvs也是版本控制系统，是集中式的，集中式的在每次写代码时都需要从服务器上拉取一份，如果服务器丢失，那么所有的都丢失，本机客户端仅仅保存当前版本信息。所有的回滚操作都需要服务器支持。
  而git是分布式的，每个电脑都是服务器，可以自由在本地回滚。

## 0.3 linux安装
```
sudo apt install git
```

# 1. 配置git环境
查看git的版本
```
git -V
```
配置：
```
git config --list
//使用q退出查看
/*
user.name   用户名
user.email  用户邮箱
http.proxy
https.proxy  端口
*/

git config -global user.name "MyName"
//其他配置同理
```
连接ssh
```
ssh -T git@github.com
//尝试连接到github
```

# 2. 仓库操作

## 2.1 创建本地仓库
```
git init
//要求该文件夹必须为空文件夹
//使用cmd命令或者linux命令进行创建
```
## 2.2  本地仓库缓存区
```
git add . 
git add --all  //所有改动文件添加到缓存区，这两行基本一样
//区别在git add . 不会记录删除操作

git commit -m "Description"  //-m参数简写提交的描述信息

git status //查看当前仓库状态  可以看到缓存区是否有文件且是否改动
```

## 2.3 提交日志
```
git log
//查看提交日志
/*
第一行 commit g2j1h8921239021  的这串符号是哈希的id，也是分布式的特色，可以用于回滚
author 是提交者
date 是提交时间
最下面是注释
*/


//如果提交操作很多，可以选择简洁显示提交日志
git log --pretty=oneline
```

## 2.4 回滚代码

```
git reset
/*
回滚有三种模式--soft --mixed --hard
*/

git reset --hard 回滚哈希id
git reset --hard HEAD~n //回滚n次
git reset --hard HEAD^  //回滚到上一次
```

git bash
git gui
git shell


git init

ssh -T git@github.com


一般的上传方式
```
git commit -m "叙述"

git push


#如果有新建文件 
git add .
```