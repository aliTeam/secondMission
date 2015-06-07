# 这个 demo 借助 express 实现了一个基本 restful 架构

## demo中用到的模块工具介绍：
1. grunt 任务自动管理工具
2. bower 前端类库管理工具
3. express nodejs的web开发框架，提供了路由控制
4. ejs 模板引擎
5. mongoose Mongodb的数据库模型工具
6. async 流程控制
7. supervisor 自动重启应用

## 服务器提供的功能
1. 提供了对数据增删操作，利用的是mongoose对mongdb操作
2. 路由控制，express的router模块
3. 模板渲染，ejs

### 笔记：
1. req.query: 处理get请求，获取get请求的参数
2. req.params: 处理类似/:xxx形式的get或者post请求，获取请求的参数
3. req.body: 处理post请求，获取post请求体
4. req.param(): 处理get和post请求，但是查找优先级为req.params->req.body->req.query
