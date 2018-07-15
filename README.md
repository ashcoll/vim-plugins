# vim as ide

## use vim8 native packages as plugin manager
## every vim plugin project is a submodule

---

### 1. 安装package（插件集）
    $ cd ~/.vim/pack/
    $ git clone --recursive git@github.com:ashcoll/vim-plugins.git

### 2. 添加插件
    $ git submodule add plugin-repo-github-addr start/submodule-name
    把插件放到~/.vim/pack/*/start/目录下，当vim启动时，这些插件会处动加载。
    建议colorscheme插件放到opt目录下；filetype plugins应放到start目录下；
    更多请参考vim文档：:h packages

### 3. 更新插件
    3.1 更新原有插件
        $ git submodule foreach git pull
    3.2 更新单个插件
        进行到子模块目录，然后执行：$ git pull
    3.3 远仓库增加了一个模块，本地需要同步
        更新模块配置信息：$ git pull
        同步新子模块到本地：$ git submodule update --init

    
---


