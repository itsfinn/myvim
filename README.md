参考自 [Vim 8内置包管理使用指南](https://blog.hulifa.cn/2019-10-20-Vim-8%E5%86%85%E7%BD%AE%E5%8C%85%E7%AE%A1%E7%90%86%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97/)

## 插件管理
添加第三方插件，比如ale

```shell
cd ~/.vim
git submoudle add git@github.com:dense-analysis/ale.git plugin/mypackage/start/ale
```

升级所有第三方插件

```shell
git submodule update --recursive --remote
```

同步vim插件到另一台机器，只需要在另一台机器上把vim插件仓库clone下来到.vim目录即可

```shell
cd ~/.vim
git clone --recursive git@github.com:itsfinn/myvim.git
```