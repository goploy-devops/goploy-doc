# SSH

## 目的
假设 A （192.168.0.1）为goploy的机器，B（192.168.0.2）为需要同步代码的机器；

A机器需要ssh免密登录B机器；

## 配置
1.登录A机器

2.执行ssh-keygen

```
[root@A 任意目录]$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/你的目录/.ssh/id_rsa):回车默认路径
Enter passphrase (empty for no passphrase):直接回车，无需密码
Enter same passphrase again:直接回车
Your identification has been saved in /你的目录/.ssh/id_rsa.
Your public key has been saved in /你的目录/.ssh/id_rsa.pub.
The key fingerprint is:
d0:82:24:8e:d7:f1:bb:9b:33:53:96:93:49:da:9b:e3 *****@******.local
```

3.将A机器.pub文件复制到B机器的 .ssh 目录

```
# A服务器运行
[root@A 任意目录]$ cat /你的目录/.ssh/id_rsa.pub
ssh-rsa
AAAAB3NzaC1yc2EAAAABIwAAAQEAlgjiMw7AskxbvpQY9rmZPQxQBzh9laxFvbaini2EgmQkNsXBA9WJOXn2YBJauoiVsdUKBWA97avjsobrTxsCYvFr1yQQvTfTlbqlqGNIhQc/3HjTl2pIkClpDWvBrRN+jpyESS4MNbfOL1qjT4c/QhGvj6U6HrN6kUyn58oyyJpTzOLG74AZELJ2Led57QvTw1yJXZuAMWioR0A3BGd25fdocLX3ebux6ya8AsloOVYfsAqGlggrARe6FXjLfMH4a/nxaAdiDYVXU/Vr1ybK9P7SfyEDGJi3JtgiPUlA6vPxUC
E+9IJPQaqqeqCGzrJ6G/XO7om1v9YLLG/H/ZN2tQ==
```
```
# 复制上面的公钥，打开B机器（最好用root登录）
[root@B 任意目录]$ 粘贴到 ~/.ssh/authorized_keys
```

4.A机器执行ssh root@192.168.0.2

## 注意
B机器authorized_keys的路径，如果不是/root/.ssh/authorized_keys，则ssh root@192.168.0.2行不通的，要换对应的用户才能连接成功。
