# vim as ide

## use vim8 native packages as plugin manager
## every vim plugin project is a submodule


### 1. 安装package（插件集）
    $ cd ~/.vim/pack/
    $ git clone git@github.com:ashcoll/vim-plugins.git

### 2. 添加插件
    $ git submodule add plugin-repo-github-addr [dir/]start
    把插件放到~/.vim/pack/*/start/目录下，当vim启动时，这些插件会处动加载。
    建议colorscheme插件放到opt目录下；filetype plugins应放到start目录下；
    更多请参考vim文档：:h packages

### 3. 更新插件
    $ git submodule foreach git pull


    



