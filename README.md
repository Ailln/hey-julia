# Hey Julia

`Julia` 语言入门。

## 1 安装

### Mac OS

去 [官网](https://julialang.org/downloads/) 下载对应的 `dmg` 文件，然后安装。

需要注意的是 Mac 安装了 Julia 后，无法直接在终端中使用 julia 命令，但是可以通过手动建立链接的形式实现，这里以 1.4 版本为例，需要根据你的版本好做调节。

```bash
ln -s /Applications/Julia-1.4.app/Contents/Resources/julia/bin/julia /usr/local/bin/julia
```

### Ubuntu

最简单的方法莫过于直接使用 apt 安装，但是这样的话版本可能会很老。比如当前最新版本是 `v1.4.2`，而使用 apt 安装的版本是 `v0.4.5`。

```bash
sudo apt install julia
```

当然你可以选择去 [官网](https://julialang.org/downloads/) 下载需要版本的压缩包，下载后直接解压。

```bash
tar -zxvf julia-1.4.2-linux-x86_64.tar.gz
```

我通常会有个专门的目录放软件，因此我们把解压后的软件移动过去。

```bash
mv julia-1.4.2 ~/software/julia-1.4.2
```

上面两个步骤你也可以直接在图像界面操作。

接下来要添加环境变量，如果你使用的是 bash 的话，操作如下（其他 shell 类似）:

```bash
$ vim ~/.bashrc
# 在底部添加
export PATH=$PATH:$HOME/software/julia-1.4.2/bin:$PATH

# 使环境生效
$ source ~/.bashrc
```

## 2 Hey

在终端中直接输入 `julia` 命令，进入 REPL 中。　

```julia
julia> println("hey julia")
hey julia

julia> name = "julia";
julia> println("hey $(name)")
hey julia
```

我们也可以在 shell 里操作，直接执行文件。

```bash
$ julia hey.jl
hey julia
hey julia
```

## 参考

- [什么是REPL？ - Ailln的回答 - 知乎](https://www.zhihu.com/question/53865469/answer/800624678)
- [Julia 中文文档](https://docs.juliacn.com/latest/)