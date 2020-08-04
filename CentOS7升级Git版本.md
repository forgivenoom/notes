# CentOS7升级(安装)Git版本
## 背景:
在 `CentOS` 上定时任务跑脚本, 执行 `git` 命令, 发现 `git` 版本过低, 官方给出的安装方式是`你TM自己编译去吧`

## 解决方案:
借助 `WANDisco` 源, 通过 `yum` 一键安装

## code:
安装wandisco源
``` shell
yum install http://opensource.wandisco.com/centos/7/git/x86_64/wandisco-git-release-7-2.noarch.rpm
```
移除老git
``` shell
yum remove git
```
安装新git
``` shell
yum install git
```

## tip:
由于使用环境不同, 可能需要sudo