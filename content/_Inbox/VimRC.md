---
date: 12-02-2024
Time: 07:44
---
" COLORS

" colorscheme

colorscheme habamax

" enable syntax highlighting

syntax enable

  

" SPACES & TABS

" set tabs to have 4 spaces

set ts=4

" indent when moving to the next line while writing code

set autoindent

" expand tabs into spaces

set expandtab

" when using the >> or << commands, shift lines by 4 spaces

set shiftwidth=4

" number of spaces in tab when editing

set softtabstop=4

  

au BufNewFile,BufRead *.py

    \ set tabstop=4

    \ set softtabstop=4

    \ set shiftwidth=4

    \ set textwidth=79

    \ set expandtab

    \ set autoindent

    \ set fileformat=unix

  

" UI CONFIG

" show line numbers

set number

" show a visual line under the cursor's current line

set cursorline

"show command in bottom bar

set showcmd

" show the matching part of the pair for [] {} and ()

set showmatch

" load filetype-specific indent files

filetype indent on

" visual autocomplete for command menu

set wildmenu

" redraw only when we neet to

set lazyredraw

" highlight matching [{()}]

set showmatch

set encoding=utf-8

" SEARCHING

" search as characters are entered

set incsearch

" highlight matches

set hlsearch

" turn off search highlight

nnoremap <leader><space> :nohlsearch<cr>

  

" FOLDING

" enable folding

set foldenable

" open most fold by default

set foldlevelstart=10

" space open/close folds

nnoremap <space> za

" fold based on indent level

set foldmethod=indent

  

" MOVEMENT

" move vertically by visual line

nnoremap j gj

nnoremap k gk

" move to beginning/end of line

nnoremap B ^

nnoremap E $

  

" Leader SHORTCUT

" leader is comma

let mapleader=","

" jk is escape

inoremap jk <esc>

" toggle gundo

nnoremap <leader>u :GundoToggle<CR>

" edit vimrc/zshrc and load vimrc bindings

nnoremap <leader>ev :vsp $MYVIMRC<CR>

nnoremap <leader>ez :vsp ~/.zshrc<CR>

nnoremap <leader>sv :source $MYVIMRC<CR>

" save session

nnoremap <leader>s :mksession<CR>

  

" CTRLP

" CtrlP settings

let g:ctrlp_match_window = 'bottom,order:ttb'

let g:ctrlp_switch_buffer = 0

let g:ctrlp_working_path_mode = 0

let g:ctrlp_user_command = 'ag %s -l --nocolor --hidden -g ""'

let g:ctrlp_user_command = 'ag %s -l --nocolor -g ""'

  

" TMUX

" allows cursor change in tmux mode

if exists('$TMUX')

    let &t_SI = "\<Esc>Ptmux;\<Esc>\<Esc>]50;CursorShape=1\x7\<Esc>\\"

    let &t_EI = "\<Esc>Ptmux;\<Esc>\<Esc>]50;CursorShape=0\x7\<Esc>\\"

else

    let &t_SI = "\<Esc>]50;CursorShape=1\x7"

    let &t_EI = "\<Esc>]50;CursorShape=0\x7"

endif

  

" AUTOGROUPS

augroup configgroup

    autocmd!

    autocmd VimEnter * highlight clear SignColumn

    autocmd BufWritePre *.php,*.py,*.js,*.txt,*.hs,*.java,*.md

                \:call <SID>StripTrailingWhitespaces()

    autocmd FileType java setlocal noexpandtab

    autocmd FileType java setlocal list

    autocmd FileType java setlocal listchars=tab:+\ ,eol:-

    autocmd FileType java setlocal formatprg=par\ -w80\ -T4

    autocmd FileType php setlocal expandtab

    autocmd FileType php setlocal list

    autocmd FileType php setlocal listchars=tab:+\ ,eol:-

    autocmd FileType php setlocal formatprg=par\ -w80\ -T4

    autocmd FileType ruby setlocal tabstop=2

    autocmd FileType ruby setlocal shiftwidth=2

    autocmd FileType ruby setlocal softtabstop=2

    autocmd FileType ruby setlocal commentstring=#\ %s

    autocmd FileType python setlocal commentstring=#\ %s

    autocmd BufEnter *.cls setlocal filetype=java

    autocmd BufEnter *.zsh-theme setlocal filetype=zsh

    autocmd BufEnter Makefile setlocal noexpandtab

    autocmd BufEnter *.sh setlocal tabstop=2

    autocmd BufEnter *.sh setlocal shiftwidth=2

    autocmd BufEnter *.sh setlocal softtabstop=2

augroup END

  

" BACKUPS

set backup

set backupdir=~/.vim-tmp,~/.tmp,~/tmp,/var/tmp,/tmp

set backupskip=/tmp/*,/private/tmp/*

set directory=~/.vim-tmp,~/.tmp,~/tmp,/var/tmp,/tmp

set writebackup

  

" split navigations

nnoremap <C-J> <C-W><C-J>

nnoremap <C-K> <C-W><C-K>

nnoremap <C-L> <C-W><C-L>

nnoremap <C-H> <C-W><C-H>

  

" CUSTOM FUNCTIONS

" toggle between number and relativenumber

function! ToggleNumber()

    if(&relativenumber == 1)

        set norelativenumber

        set number

    else

        set relativenumber

    endif

endfunc

  

" strips trailing whitespace at the end of files. this

" is called on buffer write in the autogroup above.

function! <SID>StripTrailingWhitespaces()

    " save last search & cursor position

    let _s=@/

    let l = line(".")

    let c = col(".")

    %s/\s\+$//e

    let @/=_s

    call cursor(l, c)

endfunction

  
  

" PLUGIN

  

set nocompatible              " required

filetype off                  " required

  

" set the runtime path to include Vundle and initialize

set rtp+=~/.vim/bundle/Vundle.vim

call vundle#begin()

  

" alternatively, pass a path where Vundle should install plugins

"call vundle#begin('~/some/path/here')

  

" let Vundle manage Vundle, required

Plugin 'gmarik/Vundle.vim'

  

" add all your plugins here (note older versions of Vundle

Plugin 'tmhedberg/SimpylFold'

Plugin 'vim-scripts/indentpython.vim'

Plugin 'vim-syntastic/syntastic'

Plugin 'nvie/vim-flake8'

Plugin 'scrooloose/nerdtree'

Plugin 'Lokaltog/powerline', {'rtp': 'powerline/bindings/vim/'}

" used Bundle instead of Plugin)

Bundle 'Valloric/YouCompleteMe'

let g:ycm_autoclose_preview_window_after_completion=1

map <leader>g  :YcmCompleter GoToDefinitionElseDeclaration<CR>

" ...

  

" All of your Plugins must be added before the following line

call vundle#end()            " required

filetype plugin indent on    " required

let python_highlight_all=1

  syntax on