# The-Annotated-Webbench-Sources

## 基本原理
webbench首先fork出多个子进程，每个子进程都循环做web访问测试，子进程把访问的结果通过pipe告诉父进程，父进程做最终的统计结果

## 参数说明
 * -f|--force               不需要等待服务器响应
 * -r|--reload              发送重新加载请求
* -t|--time <sec>            运行多长时间，单位：秒
 * -p|--proxy <server:port> 使用代理服务器来发送请求
* -c|--clients <n>         创建多少个客户端，默认1个"
 * 	-9|--http09              使用 HTTP/0.9 
* -1|--http10              使用 HTTP/1.0 协议
 *	-2|--http11              使用 HTTP/1.1 协议
*  --get                    使用 GET请求方法
* --head                   使用 HEAD请求方
* --options                使用 OPTIONS请求方法
* --trace                  使用 TRACE请求方法
* -?|-h|--help             打印帮助信息
* -V|--version             显示版本号
