---
hero:
  title: VIM note
  desc: dumi site app example
  actions:
    - text: Getting Started
      link: /getting-started
features:
  - icon: https://gw.alipayobjects.com/zos/bmw-prod/881dc458-f20b-407b-947a-95104b5ec82b/k79dm8ih_w144_h144.png
    title: Feature 1
    desc: Balabala
  - icon: https://gw.alipayobjects.com/zos/bmw-prod/d60657df-0822-4631-9d7c-e7a869c2f21c/k79dmz3q_w126_h126.png
    title: Feature 2
    desc: Balabala
  - icon: https://gw.alipayobjects.com/zos/bmw-prod/d1ee0c6f-5aed-4a45-a507-339a4bfe076c/k7bjsocq_w144_h144.png
    title: Feature 3
    desc: Balabala
footer: Open-source MIT Licensed | Copyright © 2020<br />Powered by [dumi](https://d.umijs.org)
---

## 安装

```shell
brew install vim
```

## 插件管理 Vim-plug

Minimalist Vim Plugin Manager

[GitHub vim-plug](https://github.com/junegunn/vim-plug)

```shell
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

## .vimrc 配置

```shell

call plug#begin('~/.vim/plugged')
Plug 'gmarik/vundle'                          " Vim Package management
Plug 'preservim/nerdtree'
Plug 'ctrlpvim/ctrlp.vim'                     " 模糊查找
Plug 'majutsushi/tagbar'                      " show tags of codes
call plug#end()
```

更多关于 [配置管理](./conf)

## Cheat Sheet

[![J3iKmt.png](https://s1.ax1x.com/2020/04/20/J3iKmt.png)](https://s1.ax1x.com/2020/04/20/J3iKmt.png)
