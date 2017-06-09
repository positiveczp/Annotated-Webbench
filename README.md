# The-Annotated-Webbench-Sources

## 基本原理
webbench首先fork出多个子进程，每个子进程都循环做web访问测试，子进程把访问的结果通过pipe告诉父进程，父进程做最终的统计结果

## 参数说明
* webbench [option]... URL
* -t ： 运行webbench的时间。
* -c ： 子进程的个数。
* -f ： 不等待返回结果。
* -h ： 帮助。

## 
