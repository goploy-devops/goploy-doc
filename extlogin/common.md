# 通用登录
提供一种自动化登录的能力，任何合法的第三方应用都可以设置goploy自动登录。举一个实际场景：当公司员工已经登录了OA系统，这时，他只需要点击一个由OA系统生成的特殊链接，便可以跳转并自动登录。

上面所说的特殊链接，其构成类似这样：

> http(s)://{{host}}/#/login?account={{account}}&token={{token}}&time={{time}}&redirect={{redirect}}

其中，用{{}}符号围起来的表示是变量。下面将用表格来说明每个变量的含义

变量名 | 必选 | 示例值 | 说明
--- | --- | --- | ---
host | 是 |domain | 部署的地址
account| 是 |  admin | 用户名
time | 是 |1921730115 | 以秒为单位的时间戳
redirect | 否 | /server/sftp | 登录成功后跳转的地址


## token生成算法

account + jwt.key + 时间戳time的字符串拼接，再进行 md5 加密

```
md5('admin' + jwt.key + '1921730115')
```