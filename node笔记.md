## node 笔记

### Buffer

* Buffer 是什么 —— 读取数据类型为Buffer，其实就是为了在JS中存储⼆进制数据
* Buffer 占用内存


### Stream流

* stream - 是⽤用于与node中流数据交互的接⼝
* http 中的 request 和 responese 其实就是流

```javascript 
const http = require('http');
const server = http.createServer((request, response) => {
    console.log('there is a request');
    response.end('a response from server');
});
```
### net
* 计算机65535个端口 ---这个数字是由于协议头只有16位用于标示合格端口，所以就只能表示2^16-1=65535个端口了


### 库


* 定制命令⾏行行界⾯面 **commander** const program = require('commander')
* 酷炫的文字工具 **figlet**
* 终端字符串美化 **chalk**
* 优雅的终端转轮 （如下载时候终端前面的转圈的动画）**ora**
* 一个用户与命令行交互的工具[inquirer](https://blog.csdn.net/qq_26733915/article/details/80461257) 
* 更全的操作文件的库**fs-extra**
