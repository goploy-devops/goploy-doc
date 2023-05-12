# 目录设计

了解各个目录的职责，这对使用该项目的时候会有个比较清晰的认知：

## Go

| 工程模块 |作用| 
|-------|--------------------|
| cmd   | 命令   |
| cmd.server   | 对外服务命令 |
| cmd.server.api   | http接口   |
| cmd.server.task   | 内置任务   |
| cmd.server.ws   | websocket接口   |
| config   | 配置文件   |
| database   | sql文件   |
| docker   | docker file   |
| internal   | 内部逻辑   |
| internal.log   | log封装   |
| internal.model   | 数据表模型   |
| internal.monitor   | 监控中心逻辑   |
| internal.pkg   | 内部共用包   |
| internal.repo   | 仓库命令封装   |
| internal.server   | 路由与响应   |
| internal.transmitter   | 文件传输封装   |
| web   | 前端项目   |

## Web.src

| 工程模块 |作用| 
|-------|--------------------|
| api   | 接口   |
| assets   | 静态资源   |
| components   | 公共组件   |
| composables   | 公共组合式函数   |
| const   | 常量   |
| icons   | svg图标   |
| lang   | 多语言   |
| layout   | 布局   |
| router   | 路由   |
| store   | vuex状态管理   |
| styles   | 样式   |
| utils   | 工具方法   |
| views   | 视图页面   |