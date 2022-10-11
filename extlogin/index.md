# Third part login

## Introduce

> http(s)://{{host}}/#/login?account={{account}}&token={{token}}&time={{time}}&redirect={{redirect}}

Var | Require | Example | Desc
--- | --- | --- | ---
host | yes |domain | app domain
account| yes |  admin | -
time | yes |1921730115 | timestamp
redirect | no | /server/sftp | redirect address


## Token algorithm

md5(account + jwt.key + timestamp)

```
md5('admin' + jwt.key + '1921730115')
```