# 远程Linux主机及进程状态监控系统---控制台子系统

## 目录

- [子系统结构](#子系统结构)
- [子系统简介](#子系统简介)
- [子系统功能说明](#子系统功能说明)
- [运行方法](#运行方法)
- [待优化内容](#待优化内容)

## 子系统结构

```text
.
├── handler              # 网站handler集
├── model                # 网站数据库操作
├── static               # 网站静态资源 
├── template             # 网页内容 
├── application.py       # 应用
├── server.py            # web服务器
├── setting.py           # 设置文件
└── urls.py              # URL地址 
```


## 子系统简介
本子系统实现添加查看监控的主机和进程状态，可对进程进行控制，完成系统的设置。


## 子系统功能说明
1. 查看关注进程的状态，包括CPU、内存、缓存和日志等内容
2. 实现便捷的进程添加

## 运行方法
```text
python server.py  # 即可，或者使用nohup命令，让程序在后台运行。使用浏览器访问
```

## 待优化内容

1. getjson函数无法做异常处理，而ajax又一直出现问题，待解决
2. 数据加密只是使用最简单的方法，可以增加关键字
3. 监控进程的子进程
5. 内存、cpu等展示页面，使用更细致的图进行展示，比如交易记录，可以拖动
7. 增加主机状态的展示

## 子系统截图


![image](https://github.com/mrcheng0910/monitoring_host_process_status/blob/master/client_monitoring/index.png)

![image](https://github.com/mrcheng0910/monitoring_host_process_status/blob/master/client_monitoring/process.png)


