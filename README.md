Pycharm golang 设置
==

### 1. 设置GOPATH环境变量
```
dbo@dbo-pc:~$ pwd
/home/dbo
dbo@dbo-pc:~$ tail -2 .profile 
# add for golang begin
export GOPATH=/home/dbo/PycharmProjects/golang
dbo@dbo-pc:~$ 
dbo@dbo-pc:~$ . .profile 
dbo@dbo-pc:~$ 
dbo@dbo-pc:~$ echo $GOPATH
/home/dbo/PycharmProjects/golang
dbo@dbo-pc:~$
```
### 2. Pycharm设置
setting --> Languages & Frameworks --> Go --> Go Libraries

添加 /home/dbo/PycharmProjects/golang（工作目录）
```
工作目录的名称是 golang
dbo@dbo-pc:~/PycharmProjects/golang$ ls -l
总用量 16
drwxrwxr-x 2 dbo dbo 4096 10月  5 17:30 bin
drwxrwxr-x 2 dbo dbo 4096 10月  5 17:30 pkg
-rw-rw-r-- 1 dbo dbo  468 10月  5 17:44 README.md
drwxrwxr-x 2 dbo dbo 4096 10月  5 17:31 src
dbo@dbo-pc:~/PycharmProjects/golang$
```
### 3. 第一个 go 程序
- MarkDown 语法表示代码快方法:
  代码块用```（代码块前后各三个）包裹起来

**经测试TAB和四个空格的方法在github不生效**

```
package main

import (
    "fmt"
)

func main() {
    fmt.Print("Hello World! 你好，世界！")
}
```
