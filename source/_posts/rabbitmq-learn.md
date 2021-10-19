---
title: rabbitmq-learn
date: 2021-10-19 17:20:29
tags:
---

#### 文档地址:  https://rabbitmq.com/getstarted.html

#### dock 安装:    
	```java 
		docker search rabbitmq;
		docker pull rabbitmq:management;
		# 运行
		# for RabbitMQ 3.9, the latest series
		docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management
		# for RabbitMQ 3.8,
		# 3.8.x support timeline: https://www.rabbitmq.com/versions.html
		docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.8-management
	```
