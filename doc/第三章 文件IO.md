# 文件I/O

## 文件描述符

**STDIN_FILENO**：标准输入文件描述符

**STDOUT_FILENO**：标准输出文件描述符

**STDERR_FILENO**：标准错误文件描述符

## 文件I/O函数

#### 打开或创建一个文件

```c
#include <fcntl.h>
int open(const char *path, int oflag, ... /* mode_t mode */);
int openat(int fd, const char *path, int oflag, ... /* mode_t mode */);
```

若成功，返回文件描述符；若出错，返回-1。

| oflag参数 | 说明                                                        |
| --------- | ----------------------------------------------------------- |
| O_RDONLY  | 只读打开                                                    |
| O_WRONLY  | 只写打开                                                    |
| O_RDWR    | 读写打开                                                    |
| O_CREAT   | 若此文件不存在则创建它                                      |
| O_TRUNC   | 如果此文件存在，而且为只写或读写成功打开，则将其长度截断为0 |

```c
#include <fcntl.h>
int creat(const char *path, mode_t mode);
/* 相当于 */
open(path, O_WRONLY | O_CREAT | O_TRUNC, mode);
```

若成功，返回为只写打开的文件描述符；若出错，返回-1。

#### 关闭一个打开文件

```c
#include <unistd.h>
int close(int fd);
```

#### 显示的为一个打开文件设置偏移量

```c
#include <unistd.h>
off_t lseek(int fd, off_t offset, int whence);
```

若成功，返回新的文件偏移量；若出错，返回-1。

#### 从打开的文件中读数据

```c
#include <unistd.h>
ssize_t read(int fd, void *buf, size_t nbytes);
```

返回值：读到的字节数，若已到文件尾，返回0；若出错，返回-1。

#### 向打开的文件写数据

```c
#include <unistd.h>
ssize_t write(int fd, const void *buf, size_t nbytes);
```

返回值：若成功，返回已写的字节数；若出错，返回-1。



