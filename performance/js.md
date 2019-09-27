# js

### 1. JS放body尾部，JS，CSS都需要放在head中时，JS放在前面

* CSS会阻塞页面的渲染，不阻塞DOM的解析；
* JS会阻塞DOM的解析，但是，浏览器会预先下载资源；
* 浏览器在遇到script标签时会触发页面渲染，如果这时CSS尚未加载完成，页面将会等待CSS加载完成后在执行；

### 2. 利用`setTimeout`代替`setInterval`

`setInterval`可能存在指令堆积的问题，导致页面卡顿。

### 

