**ln指令**

> 软链接也成为符号链接，类似于windows里的快捷方式，主要存放了链接其他文件的路径这不是大写的i 而是大写是L的l

基本语法

```text
In -s [原文件或目录] [软链接名] （功能描述：给原文件创建一个软链接）
```

在/home目录下创建一个软连接linkToRoot，连接到/root目录

```
ln -s /home linkToHome
cd linkToHome
```

**history指令**

查看已经执行过历史命令，也可以执行历史指令基本语法

```text
history（功能描述：查看已经执行过历史命令）
```

**搜索查找类**

**find指令**

> find指令将从指定目录向下递归地遍历其各个子目录，将满足条件的文件或者目录显示在终端。

基本语法

```text
find [搜索范围] [选项]
```

选项说明

![img](https://pic3.zhimg.com/80/v2-e3a3f24889c025939bb16b9fd18b4346_1440w.jpg)

按文件名：根据名称查找/home目录下的a.txt文件

![img](https://pic2.zhimg.com/80/v2-4d86d9bb3878a40de6ce2b131f757465_1440w.jpg)

> 第二个参树是搜索的范围 -name 按照文件名 最后一个是文件按拥有者：查找/home目录下，用户名称为root的文件

![img](https://pic4.zhimg.com/80/v2-9ce68e23d16e71d051ad0a5d78319cdb_1440w.jpg)

> 查找整个linux系统下大于200m的文件（+n大于 -n小于 n等于）

![img](https://pic3.zhimg.com/80/v2-65fbd44a2dc65b65954550ffde866372_1440w.jpg)

查询/home 目录下所有以.txt结尾的文件

![img](https://pic3.zhimg.com/80/v2-059c1964843b5ec83f6984353bd3766a_1440w.jpg)

**locate指令**

> locaate指令可以快速定位文件路径。
> locate指令利用事先建立的系统中所有文件名称及路径的locate数据库实现快速定位给定的文件。
> Locate指令无需遍历整个文件系统，查询速度较快。为了保证查询结果的准确度，管理员必须定期更新locate时刻。

基本语法

```text
locate 搜索文件
```

**grep指令和管道符号 |**

> 管道符号的l是小写的字母哈grep过滤查找，管道符，“l”，表示将前一个命令的处理结果输出传递给后面的命令处理。基本语法

```text
grep [选项] 查找内容源文件
```

常用选项

![img](https://pic1.zhimg.com/80/v2-8f8ce5ca91640007cbf5e27d8acd39b4_1440w.jpg)

在bbb.txt文件中照抄dfa

![img](https://pic4.zhimg.com/80/v2-b4591e61f1e196a2854229b0c68f7c1f_1440w.jpg)

cat bbb.txt 取得文件内容，然后交给了后面的grep dfa进行后面的操作。

