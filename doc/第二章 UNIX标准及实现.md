# UNIX标准及实现

## UNIX  标准

#### ISO C

提供C程序的可移植性，使其能适合于大量不同的操作系统，而不只是适合UNIX系统。此标准不仅定义了C程序设计语言的语法和语义，还定义了其标准库。

| 头文件       | 说明                     |
| ------------ | ------------------------ |
| <assert.h>   | 验证程序断言             |
| <complex.h>  | 复数算术运算支持         |
| <ctype.h>    | 字符分类和映射支持       |
| <errno.h>    | 出错码                   |
| <fenv.h>     | 浮点环境                 |
| <float.h>    | 浮点常量及特性           |
| <inttypes.h> | 整型格式变换             |
| <iso646.h>   | 赋值、关系及一元操作符宏 |
| <limits.h>   | 实现常量                 |
| <locale.h>   | 本地化类别及相关定义     |
| <math.h>     | 数学函数、类型声明及常量 |
| <setjmp.h>   | 非局部goto               |
| <signal.h>   | 信号                     |
| <stdarg.h>   | 可变长度参数表           |
| <stdbool.h>  | 布尔类型和值             |
| <stddef.h>   | 标准定义                 |
| <stdint.h>   | 整型                     |
| <stdio.h>    | 标准I/O库                |
| <stdlib.h>   | 实用函数                 |
| <string.h>   | 字符串操作               |
| <tgmath.h>   | 通用类型数学宏           |
| <time.h>     | 时间和日期               |
| <wchar.h>    | 扩充的多字节和宽字符支持 |
| <wctype.h>   | 宽字符分类和映射支持     |

#### POSIX

由IEEE制定的可移植操作系统接口(Portable Operating System Interface)。

| 头文件          | 说明                 |
| --------------- | -------------------- |
| <aio.h>         | 异步I/O              |
| <cpio.h>        | cpio归档值           |
| <dirent.h>      | 目录项               |
| <dlfcn.h>       | 动态链接             |
| <fcntl.h>       | 文件控制             |
| <fnmatch.h>     | 文件名匹配类型       |
| <glob.h>        | 路径名模式匹配与生成 |
| <grp.h>         | 组文件               |
| <iconv.h>       | 代码集变换实用程序   |
| <langinfo.h>    | 语言信息常量         |
| <monetary.h>    | 货币类型与函数       |
| <netdb.h>       | 网络数据库操作       |
| <nl_types.h>    | 消息类               |
| <poll.h>        | 投票函数             |
| <pthread.h>     | 线程                 |
| <pwd.h>         | 口令文件             |
| <regex.h>       | 正则表达式           |
| <sched.h>       | 执行调度             |
| <semaphore.h>   | 信号量               |
| <strings.h>     | 字符串操作           |
| <tar.h>         | Tar归档值            |
| <termios.h>     | 终端I/O              |
| <unistd.h>      | 符号常量             |
| <wordexp.h>     | 字扩充类型           |
| <arpa/inet.h>   | 因特网定义           |
| <net/if.h>      | 套接字本地接口       |
| <netinet/in.h>  | 因特网地址族         |
| <netinet/tcp.h> | 传输控制协议定义     |
| <sys/mman.h>    | 存储管理声明         |
| <sys/select.h>  | select函数           |
| <sys/socket.h>  | 套接字接口           |
| <sys/stat.h>    | 文件状态             |
| <sys/statvfs.h> | 文件系统信息         |
| <sys/times.h>   | 进程时间             |
| <sys/types.h>   | 基本系统数据类型     |
| <sys/un.h>      | UNIX域套接字定义     |
| <sys/utsname.h> | 系统名               |
| <sys/wait.h>    | 进程控制             |

#### Single UNIX Specification（SUS,单一UNIX规范）

POSIX.1标准的超集，定义了一些附加接口扩展了POSIX.1规范提供的功能，只有遵循XSI的实现才能称为UNIX系统。

## UNIX  实现

| 实现     | 说明                                 |
| -------- | ------------------------------------ |
| SVR4     | AT&T的UNIX系统实验室                 |
| 4.4BSD   | 加州大学伯克利分校的计算机系统研究组 |
| FreeBSD  | 4.4BSD-Lite                          |
| Linux    | Linus Torvalds                       |
| Mac OS X | Darwin                               |
| Solaris  | Sun Microsystems开发的UNIX系统版本   |

