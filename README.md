
使用 pathogen + git 管理 Vim 插件，参考 [教程：使用 pathogen + git 管理 Vim 插件](http://lostjs.com/2012/02/04/use-pathogen-and-git-to-manage-vimfiles/)

## 使用

`git clone` 后，使用 `git submodule update --init --recursive` 初始化插件

### 安装插件

```bash
git submodule add git://github.com/XXX/XXX.git bundle/XXX
```

### 升级插件

```bash
git checkout master; git pull
```

批量升级

```bash
git submodule foreach 'git checkout master && git pull'
```

### 删除插件

```bash
rm -rf bundle/XXX
git rm -r bundle/XXX
```

## 插件介绍

- [vim-multiple-cursors](https://github.com/terryma/vim-multiple-cursors): 多选批量操作。使用：`ctrl + n`
- [nerdtree](https://github.com/scrooloose/nerdtree): 
tree explorer。使用：`:NERDTreeToggle`