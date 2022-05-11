# sftp
SFTP (SSH File Transfer Protocol) is a secure file transfer protocol. It runs over the SSH protocol. It supports the full security and authentication functionality of SSH.

## Grammar

```
rsync [OPTION]... SRC DEST
```

## Notice
Goploy will automatically fill SRC and DES

## Option

```
-v increase verbosity.
--exclude=PATTERN exclude file equal to PATTERN.
--exclude-regexp=REGEXP exclude files matching PATTERN.
--include=PATTERN don't exclude file equal to PATTERN.
--include-regexp=REGEXP don't exclude files matching PATTERN.
```
