# sftp命令

SFTP（Secure File Transfer Protocol，安全文件传输协议）是一种基于可靠数据流（data stream），提供文件存取和管理的网络传输协议。

## 语法

```
sftp  [OPTION]... SRC DEST
```

## 注意
Goploy会在程序中自动拼接SRC和DES

## 选项

```
-v 详细模式输出
--exclude=FILE 指定排除不需要传输的文件
--include=FILE 指定不排除而需要传输的文件
--exclude-regexp=REGEXP 排除正则表达式中匹配的文件
--include-regexp=REGEXP 不排除正则表达式匹配的文件
```
