## 概述

工具名称为蝙蝠工具箱(BatBox)，作者为永恒之锋Gu0st开发，必须联合bat文件才能运行，自动爬取同目录和子目录下的所有bat文件

此工具为bat工具箱，因为任何脚本均可用bat调用，在作者的想法下，想到利用调用bat文件实现工具箱的功能。原想法就是在自己电脑中有一个专门的文件，里面保存了各种工具，又不想一个一个打开退出，所以才想到这个办法。

## bat命令

### 替换加粗部分

2023.9.4更新

为了让小白也可以利用此工具，特此附上简单的bat命令

```
@echo off
cd /d %~dp0
start cmd /K "chcp 65001&&python 1.py --help "
```

替换为python **1.py** --help，或者替换整条命令如：**java -jar xxx.jar**

2023.9.6更新

针对**exe**可执行文件，去掉cmd黑框的bat命令

```
@echo off
cd /d %~dp0
start /min "" cmd /C "chcp 65001 &&start zenmap.exe"
```

替换为**zenmap.exe**

chcp 65001是设置命令行界面为utf-8，方便查看中文信息。

2025年1月16日更新
<img width="491" alt="e482a29aaf87ea39702b0ad02b59400" src="https://github.com/user-attachments/assets/9794c081-d66e-4887-989c-141f25935b72" />


## 总结

工具配置好了会特别方便 ，电脑随便乱搞，随走随带

如果当前路径下无bat文件，将会显示空白

关注永恒之锋
<p align="center">
  <img src="https://lit.enomothem.com/zhixinghe/20220528141025.jfif">
</p>
