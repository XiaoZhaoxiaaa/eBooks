# eBook分享大集合

- 主要以IT领域经典书籍收藏，以备不时之需。
- - [x] 表示文件大小超过100M。

## 服务器系统类

> 1. Linux高性能服务器编程
> 2. Shell脚本学习指南
> 3. 鸟哥的Linux私房菜基础篇第三版
> 4. 深入理解计算机系统

## 机器学习类

> 1. 吴恩达深度学习教程
> 2. deepLearning深度学习_开源版
> 3. python自然语言处理实战：核心技术与算法
> 4. 机器学习方法
> 5. 统计学习方法
> 6. 用Python进行自然语言处理

## 算法类

> 2. 编程之法面试和算法心得
> 3. 编程珠玑(第2版)
> 4. 大话数据结构
> 4. 数据结构(C语言版).严蔚敏_吴伟民.扫描版

## 网络类

> 1. 图解TCP IP(第5版)

## 程序语言类

#### C/C++语言
> 1. C++ Primer第五版中文版
> 2. C语言程序设计
> - [x] 3. C语言入门经典(第四版).（美）霍顿
> 4. modern-cpp-tutorial
> 5. 大规模C++程序设计

#### Python语言

> 1. Python.Cookbook(第2版)中文版
> 2. Python标准库中文版
> 3. Python高级编程（法莱德）.扫描版
> 4. Python核心编程(第2版)
> 5. Python灰帽子
> 6. python基础教程(第2版)
> 7. Python源码剖析
> 8. 编写高质量代码 改善Python程序的91个建议
> 9. 利用Python进行数据分析
> 10. 流畅的Python

#### Java语言

> 1. Java编程思想(第4版)完整版
> 2. Java入门经典
> 3. 设计模式之禅完整版 秦晓波

#### PHP语言

> - [x] 1. PHP 核心技术与最佳实践
> 2. PHP与MYSQL权威指南
> 3. PHP高级程序设计_模式、框架与测试

#### C#/.NET语言

> 1. .NET本质论
> 2. .NET应用程序架构设计 原则 模式与实践
> 3. ASP.NET MVC4 WEB编程
> 4. ASP.NET MVC4高级编程
> 5. ASP.NET MVC4框架揭秘
> 6. ASP.NET.4.0 揭秘(卷1)
> 7. ASP.NET.4.0 揭秘(卷2)
> 8. ASP.NET本质论
> 9. C#本质论
> 10. C#程序开发范例宝典
> - [x]  11. C#范例开发大全
> 12. C#高级编程（第7版）
> - [x] 13. C#核心开发技术从入门到精通
> 14. C#入门经典(第3版)
> 15. C#入门经典(第5版)
> 16. C#与.NET程序员面试宝典.靳华.胡鑫鑫.扫描版
> 17. CLR.via.C#（第3版）
> 18. WCF全面解析（上册）
> 19. WCF全面解析（下册）
> 20. 编写高质量代码改善C#程序的157个建议
> 21. 大话设计模式

#### Web技术

> 1. CSS权威指南(第3版)
> 2. HTML5权威指南
> 3. HTTP权威指南
> 4. JavaScript权威指南(第4版)
> 5. JavaScript权威指南(第6版)
> 6. jQuery权威指南
> 7. WebKit技术内幕(朱永盛著)
> - [x] 8. 锋利的jquery
> 9. 高性能网站建设进阶指南

## 数据库类

#### Oracle

> - [x] 1. Oracle+Database+11g数据库管理艺术
> 2. PLSQL操作手册
> 3. 编程艺术深入数据库体系结构
> 4. 剑破冰山  Oracle开发艺术
> 5. 收获，不止Oracle

#### MySQL

> 2. MySQL 5权威指南  （第3版）
> 3. MYSQL必知必会
> 4. MySQL技术内幕(第4版) 
> 4. MySQL技术内幕：SQL编程（姜承尧）
> 5. MySQL技术内幕InnoDB存储引擎
> 6. 高性能MySQL_第3版（中文）

#### SQL Server

> - [x] 1. SQL Server企业级平台管理实践
> 2. SQL2005技术内幕： T-SQ程序设计
> 3. SQL2005技术内幕：存储引擎
> 4. SQL2008技术内幕：T-SQL查询
> 5. SQL2008技术内幕：T-SQL语言基础
> 6. SQLServer2008查询性能优化
> 7. SQL反模式中文完整版
> 8. Transact-SQL权威指南
> - [x] 9. 大话数据库

## 其他类

> 1. 程序员的自我修养—链接、装载与库
> 2. 代码整洁之道.(美)马丁
> 3. 人月神话中文版

## 非书籍类

> 1. C语言学习资料.exe

# GitHub上传100M以上文件解决方案

- 工具下载，详见[【官网】](https://git-lfs.github.com/)

> [git-lfs-windows](https://github.com/git-lfs/git-lfs/releases/download/v2.8.0/git-lfs-windows-v2.8.0.exe)
> [git-lfs-mac](https://github.com/git-lfs/git-lfs/releases/download/v2.8.0/git-lfs-darwin-amd64-v2.8.0.tar.gz)

- 基本步骤及其命令

```shell
# 在项目中安装lfs
$ git lfs install
# 需要push的文件
$ git lfs track "程序语言类\C&C++语言\C语言入门经典(第四版).（美）霍顿.pdf"
$ git add .gitattributes
$ git lfs track "程序语言类\C&C++语言\C语言入门经典(第四版).（美）霍顿.pdf"
$ git add "程序语言类\C&C++语言\C语言入门经典(第四版).（美）霍顿.pdf"
$ git commit -m "[add] add lfs ebook for C."
$ git push origin master
```