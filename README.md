---
description: 主要记录一下在Mac 上的安装配置
---

# 安装

MAC 系统一般都自带有 Python2.x 版本的环境，不过现在都不用 2.x 的版本了，所以建议你在 [https://www.python.org/downloads/mac-osx/](https://www.python.org/downloads/mac-osx/) 上下载最新版安装。

安装完成之后，如何配置环境变量呢？

先查看当前环境变量：

```text
echo $PATH
```

然后打开 `~/.bash_profile(没有请新建 touch .bash_profile)`

可以使用 vi 工具打开并编辑该文件，也可以直接打开.bash\_profile文件，使用`open .bash_profile`

```text
vi ~/.bash_profile
** 或者 **
open .bash_profile
```

我装的是 Python3.9 ，Python 执行路径为：`/Library/Frameworks/Python. Framework/Versions/3.9/bin` 。于是写入

```text
export PATH="/Library/Frameworks/Python. Framework/Versions/3.9/bin:$PATH"
```

最后保存退出，激活运行一下文件：

```text
source ~/.bash_profile
```



