# 压缩/解压缩

## **tar.gz**

### 在不解压缩的情况下，查看包内的文件信息 

```bash
tar -ztvf file.tar.gz
```

参数：

```bash
-z, --gzip, --gunzip, --ungzip    filter the archive through gzip
-t, --list                        list the contents of an archive
-v, --verbose                     verbosely list files processed
-f, --file=ARCHIVE                use archive file or device ARCHIVE
```

from: https://www.cnblogs.com/0820LL/p/9620158.html

### 在不解压缩的情况下，查看文件压缩前后的整体大小、压缩率

```bash
gzip -l file.tar.gz
```

### 解压到指定文件夹

使用 参数`-C`

```
tar -ztvf form5500_pack.tar.gz form5500_pack/folder
```

### 解压指定文件

查看所需解压的文件存不存在

```
tar -ztvf form5500_pack.tar.gz | grep 'f_sch_r_part1_09_17.sas7bdat'
```

然后解压该文件

```
tar -ztvf form5500_pack.tar.gz form5500_pack/f_sch_r_part1_09_17.sas7bdat
```







# 把输出写入到文件

### 只保存在文件中

只输出到指定文件（如已存在，覆盖原文件）

```bash
ls > file.text	
```

只输出到指定文件的后面（如已存在，保留原文件）

```bash
ls >> file.text
```

### 终端输出 & 记录在文件

屏幕打印输出信息并记录到文件中

使用指令`tee`: read from standard input and write to standard output and files

```bash
ls | tee file.txt

```

屏幕打印输出信息并记录到文件中（保留原文件内容）

使用参数 `-a, --apend`

### 记录多个命令的输出

启动命令：`script`		*默认自动记录到typescript文件中*

启动命令 & 指定文件名：`script -a file.txt`		*默认自动记录到typescript文件中*

终止命令：`exit`

```

```

