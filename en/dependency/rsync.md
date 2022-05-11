# rsync
rsync -- a fast, versatile, remote (and local) file-copying tool

## Grammar

```
rsync [OPTION]... SRC DEST
rsync [OPTION]... SRC [USER@]host:DEST
rsync [OPTION]... [USER@]HOST:SRC DEST
rsync [OPTION]... [USER@]HOST::SRC DEST
rsync [OPTION]... SRC [USER@]HOST::DEST
rsync [OPTION]... rsync://[USER@]HOST[:PORT]/SRC [DEST]
```

## Notice
Goploy will automatically fill SRC and DES

[rsync man page](https://linux.die.net/man/1/rsync)