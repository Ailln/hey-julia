# Hey Julia

`Julia` 语言入门。

## 1 Hey

使用 Julia 的 REPL：

```julia
julia> println("hey julia")
hey julia

julia> name = "julia";
julia> println("hey $(name)")
hey julia
```

在 shell 里操作：

```bash
$ julia hey.jl
hey julia
hey julia
```

## 注意

Mac 安装了 Julia 后，无法直接在终端中使用 julia 命令，但是可以通过手动建立链接的形式实现，这里以 1.4 版本为例，需要根据你的版本好做调节。

```bash
ln -s /Applications/Julia-1.4.app/Contents/Resources/julia/bin/julia /usr/local/bin/julia
```
