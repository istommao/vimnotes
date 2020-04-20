# 配置管理 .vimrc

```shell
"侦测文件类型"
filetype on
"载入文件类型插件"
filetype plugin on
"为特定文件类型载入相关缩进文件"
filetype indent on

"自动开启语法高亮"
syntax enable

"当文件在外部被修改时，自动更新该文件"
set autoread

call plug#begin('~/.vim/plugged')
Plug 'gmarik/vundle'                          " Vim Package management
Plug 'preservim/nerdtree'
Plug 'mattn/emmet-vim'                        " zen coding
Plug 'mattn/webapi-vim'
" Plug 'mattn/gist-vim'
Plug 'airblade/vim-gitgutter'                 " git diff
Plug 'vim-airline/vim-airline'
Plug 'Yggdroot/indentLine'
Plug 'vim-airline/vim-airline-themes'
Plug 'scrooloose/nerdcommenter'               " Quick comment
Plug 'ctrlpvim/ctrlp.vim'                     " 模糊查找
Plug 'terryma/vim-multiple-cursors'           " 多光标编辑
Plug 'tpope/vim-fugitive'                     " git插件 （Blame)
" Plug 'godlygeek/tabular'                      " 自动根据某个符号对其，用于json 字典 表格等
Plug 'tweekmonster/startuptime.vim'           " Vim start up time debug (figure out which script is slow)
Plug 'dyng/ctrlsf.vim'                        " Ascyn use rg to find
Plug 'majutsushi/tagbar'                      " show tags of codes
" Plug 'Vimjas/vim-python-pep8-indent'          " auto indent ()
" Plug 'tweekmonster/django-plus.vim'
Plug 'spacewander/openresty-vim'
Plug 'kien/rainbow_parentheses.vim'           " Rainbow Parentheses
Plug 'cespare/vim-toml'
Plug 'stephpy/vim-yaml'
Plug 'nvie/vim-flake8'
Plug 'mxw/vim-jsx'
Plug 'prabirshrestha/async.vim'               " Async complete with vim-lsp
Plug 'prabirshrestha/asyncomplete.vim'
Plug 'mzlogin/vim-markdown-toc'
Plug 'gabrielelana/vim-markdown'
Plug 'benmills/vimux'
Plug 'flazz/vim-colorschemes'
Plug 'dense-analysis/ale'

" post install (yarn install | npm install) then load Plug only for editing supported files
Plug 'prettier/vim-prettier', {
  \ 'do': 'yarn install',
  \ 'for': ['javascript', 'typescript', 'css', 'less', 'scss', 'json', 'graphql', 'markdown', 'vue', 'html'] }

call plug#end()


"显示标尺"
set ruler

"显示行数"
set nu
" set foldmethod=indent
set nofoldenable               " disable folding
set mouse=a                    " 支持鼠标

"设置所有的Tab和缩进为4个空格"
set tabstop=4

"设定<<和>>命令移动时的宽度为4"
set shiftwidth=4

"使得按退格键时可以一次删除4个空格"
set softtabstop=4
set smarttab

"使用空格来替换Tab"
set expandtab

" filetype indent on

set autoindent
set smartindent
set shiftround

" General settings --------------------{{{
set encoding=utf-8
let mapleader=','
syntax enable


let g:indentLine_concealcursor = 'inc'
let g:indentLine_conceallevel = 2

" let g:indentLine_char = '┆'
let g:indentLine_char_list = ['|', '¦', '┆', '┊']
let g:indentLine_enabled = 1
let g:indentLine_color_term = 50

" 设置NerdTree

map <F3> :NERDTreeMirror<CR>
map <F3> :NERDTreeToggle<CR>
```
