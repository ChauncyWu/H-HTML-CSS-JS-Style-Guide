# html

### 1. 注重标签的语义化，保持用最简洁的标签完成所需的功能

标签的语义化提高代码的可维护性，在页面加载CSS失败时也不至于很难看。同时，需要保持标签最小化，无意义的标签可以利用伪类表示。

### 2. 尽量避免使用iframe

iframe 内资源的下载进程会阻塞父页面静态资源的下载与 CSS 及 HTML DOM 的解析。

### 3. HTML代码压缩，去除注释、空白符

