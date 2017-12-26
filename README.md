# Rust 程序设计语言（第二版） 简体中文版

还在施工中：目前翻译到第十六章，正在更新第十二章

目前官方进度：[第十七章](https://github.com/rust-lang/book/projects/1)（18~20 章还在编写当中）

GitBook 代码排版已大体解决，已不影响阅读


### Requirements

构建本书需要使用[mdBook](https://github.com/azerupi/mdBook)

```shell
$ cargo install mdbook --vers [version-num]
```

### 构建

在根目录执行：

```shell
$ mdbook build
```

构建文件在mdbook子目录，使用浏览器打开：

*FireFox:*

```shell
$ firefox mdbook/index.html                       # Linux
$ open -a "Firefox" mdbook/index.html             # OS X
$ Start-Process "firefox.exe" .\mdbook\index.html # Windows (PowerShell)
$ start firefox.exe .\mdbook\index.html           # Windows (Cmd)
```

*Chrome:*

```shell
$ google-chrome mdbook/index.html                 # Linux
$ open -a "Google Chrome" mdbook/index.html       # OS X
$ Start-Process "chrome.exe" .\mdbook\index.html  # Windows (PowerShell)
$ start chrome.exe .\mdbook\index.html            # Windows (Cmd)
```

### mdbook发布到gh-pages分支

```shell
$ git subtree push --prefix mdbook origin gh-pages
```