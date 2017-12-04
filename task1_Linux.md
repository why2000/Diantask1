# 熟悉Linux操作系统及基本操作指令

[Day4]

* * *

## 本日进度

### 1. 通过[鳥哥的 Linux 私房菜 -- 第十章、認識與學習BASH](http://linux.vbird.org/linux_basic/0320bash.php)复习/学习了Linux的常用操作指令

1. 基于 `Ubuntu Kylin on VMware Workstation(version 16.04)` Bash shell
2. 新学习的指令:
    * alias(built-in):
        1. 输入`alias name1=command`可为command指定别名name1
        2. 直接输入`alias`，可查看当前已设置的别名列表
        3. 输入`unalias name1` 可删除已设置的别名
    * type(built-in):
        1. 输入`type name`可查看name是外部指令还是内建指令
        2. 作为内建指令使用help type后可查看使用参数
        3. 实用参数: 
            * `-a` 可查看有多种别名的name的所有用法
            * `-t` 用几种简称来表示name的用法
            * `-p` 仅返回对应简称为file的用法的信息
    * date(file):
        1. 可用于输出当前日期
        2. 输出格式调整的方式可用`date --help`查看
    * cal(file):
        1. 可用于输出日历(cal [month] [year])
        2. 输出格式调整帮助会在输入错误指令(如cal --help)后被输出
    * apropos
3. 了解了新功能的指令: