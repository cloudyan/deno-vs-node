# deno-vs-node

Deno VS Node

     vs     |        Node       |     Deno
----------- | ----------------- | --------------
API 引用方式  | 模块导入           | 全局对象
模块系统      | CommonJS & 新版 node 实验性 ES Module | ES Module 浏览器实现
安全         | 无安全限制          | 默认安全
Typescript   | 第三方，如通过 ts-node 支持 | 原生支持
包管理        | npm + node_modules | 原生支持
异步操作      | 回调              | Promise
包分发        | 中心化 npmjs.com  | 去中心化 import url
入口          | package.json 配置 | import url 直接引入
打包、测试、格式化  | 第三方如 eslint、gulp、webpack、babel 等 | 原生支持

1. 内置 API 引用方式不同
2. 模块系统
     - node 采用的是CommonJs规范
     - deno 完全遵循 ES Module 的浏览器实现
       - 可以通过 import url 直接引用线上资源
       - 资源不可省略扩展名和文件名
3. 安全
     - 默认安全的 deno
     - 白名单
4. 兼容浏览器 API
     - 概念上兼容
     - 存在 window 全局变量
     - 实现了 WindowOrWorkerGlobalScope 的全部方法
5. 支持 Typescript
6. 去 node_modules
     - Download 和 Compile
7. 标准模块 与 node API 兼容
8. 异步操作
9. 单文件分发
10. 去中心化仓库
    - deno 其实是有个基于 GitHub 的[第三方模块集合](https://deno.land/x)。
11. 去开发依赖

参考：

- https://www.cnblogs.com/coderhf/p/12911812.html
