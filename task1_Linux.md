# 熟悉Linux操作系统及基本操作指令

[Day4]

* * *

## 本日进度

### 1. 通过[鳥哥的 Linux 私房菜 -- 第十章、認識與學習BASH](http://linux.vbird.org/linux_basic/0320bash.php) 及其 [第四章](http://linux.vbird.org/linux_basic/0160startlinux.php#cmd_hkey) 中复习/学习了Linux的常用操作指令

1. 基于 `Ubuntu Kylin on VMware Workstation(version 16.04)` Bash shell
2. 新学习的指令:
    * alias(built-in):
        1. 使用 `alias name1=command` 可为command指定别名name1
        2. 直接使用 `alias` ，可查看当前已设置的别名列表
        3. 使用 `unalias name1` 可删除已设置的别名
    * type(built-in):
        1. 输入`type name` 可查看name是外部指令还是内建指令
        2. 作为内建指令使用 `help type` 后可查看可用参数
        3. 实用参数: 
            * `-a` 可查看有多种别名的name的所有用法
            * `-t` 用几种简称来表示name的用法
            * `-p` 仅返回对应简称为file的用法的信息
    * date(file):
        1. 可用于输出当前日期
        2. 输出格式调整的方式可用 `date --help` 查看
    * cal(file):
        1. 可用于输出日历( `cal [month] [year]` )
        2. 输出格式调整帮助会在输入错误指令(如 `cal --help` )后被输出
    * apropos(file):
        1. 可用于查找名称或描述中包含某段关键字的所有指令
        2. 使用参数 `-e` 可仅搜索将关键字作为一个单词存在与名称或描述中的指令
    * uniq(file):
        1. 使用 `uniq filein fileout` 报告或忽略文件中的重复行
        2. 使用 `uniq --help` 后可查看可用参数
        3. 实用参数:
            * `-u` 仅保留只出现过一次的行
            * `-d` 仅保留重复出现过的行
            * `-c` 显示某行出现的次数

* * *

[Day5]

* * *

## 本日进度

### 进行各指令的功能复习:

* 各指令功能概述如下：
 > man（显示使用手册）, ls（显示目录下的项）, mkdir（创建目录）, cd（切换目录）, cp（本地复制文件）, scp（远程复制文件）, ssh（指定ssh加密协议）, rm（删除文件）, netstat（显示网络信息）, ps（显示进程）, top（查看系统运行情况）, ifconfig（配置网络）, cat（查看文件）, head, tail, less（增强型cat）, more（削弱型less）, echo（输出）, date（显示日期）, vi（文本编辑器）, vim（增强版vi）, nano（文本编辑器）, wget（下载网络文件）, curl（下载/上传）, mv（移动文件/重命名）, chmod（更改权限）, chgrp（切换用户组）, chown（改变所有者）, passwd（密码相关）, sudo（root权限）, touch（更新文件时间）, grep（搜索文本）, find（搜索文件）, locate（高速版find）, cut（分割文件）, sort（排序文件内容）, wc（统计文件内容）, awk（文件按行切片读取）, uniq（重复行检索）, paste（连接文件）, systemd（系统启动）, systemctl（系统运行参数修改）