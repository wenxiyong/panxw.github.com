---
layout: post
category: "javaDesign"
title:  "并发场景"
tags: [github, jekyll]
---
- [ ] 	库分表分库

- 订单分表分库思路 
- - 分库： 二叉树分库
- - 分表：
- - 数据库目标索引：   
- - - 数据库编号 = （userId / tableCount） % databaseCount    
- - - 表编号 = userId % tableCount
- - 访问方式：
- - - 客户端负责索引，直接连接数据库查询指定库跟指定表
- - - 利用数据库中间件 
- - - 相关产品：
- - - - [Mycat](http://www.mycat.io/)
- - - - [芒果](https://github.com/jfaster/mango)


