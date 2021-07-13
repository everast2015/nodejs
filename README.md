# nodejs 学习笔记

## 进程和线程的关系

- 进程为程序的运行提供必备的环境
- 进程就相当于工厂中的车间

线程：

- 线程计算机中最小的计算单位，线程负责进程中执行的程序
- 线路就相当于工厂中的工人

单线程和多线程：

- js 是单线程，相当于一个人干活
- 多线程，相当于多个人一起干活


## 模块化概念

1. 在nodejs中，引入文件的路径，必须是以`./`或者`../` 相对路径的形式进行引入。
2. 在nodejs中，如果引入的文件的路径是没有`./`或者 `../`，那么默认去`node_modules` 依赖包里面去查找。
3. 在nodejs中，一个js文件就是一个模块
4. 每一个js文件中的代码，都是独立运行在一个函数当中，而不是全局作用域，所以一个模块中的变量和函数在其他模块中，无法访问。


如何解决js中的模块不能互相访问的问题：

1. 此时需要导出模块，此时可以使用关键词 `export` 导出模块
2. 向外部暴露属性的方法
