# web-worker-study
Web Worker study


## 为什么javascript是单线程

作为浏览器脚本语言，JavaScript的主要用途是与用户互动，以及操作DOM。这决定了它只能是单线程，否则会带来很复杂的同步问题。比如，假定JavaScript同时有两个线程，一个线程在某个DOM节点上添加内容，另一个线程删除了这个节点，这时浏览器应该以哪个线程为准？

## web worker 限制

 - worker.js必须跟index.html是同域的，且无法是本地的静态文件目录(无法识别 `file://` 这种地址)