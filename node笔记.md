## node 笔记

### Buffer

* Buffer 是什么 —— 读取数据类型为Buffer，其实就是为了在JS中存储⼆进制数据
* Buffer 占用内存


### Stream流

* stream - 是⽤用于与node中流数据交互的接⼝
* http 中的 request 和 responese 其实就是流

```javascript const http = require('http');
const server = http.createServer((request, response) => {
    console.log('there is a request');
    response.end('a response from server');
});
```

### 库

* 定制命令⾏行行界⾯面 **commander** const program = require('commander')
* 酷炫的文字工具 **figlet**
* 终端字符串美化 **chalk**
* 优雅的终端转轮 （如下载时候终端前面的转圈的动画）**ora**
* 