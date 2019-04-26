# dotfiles


cat ~/.config/nvim/init.vim 
https://github.com/mauroporrasp/dotfiles



" David's commands
```
"nnoremap <Leader>f :RangerEdit<CR>
vnoremap > >gv
vnoremap < <gv
set nowrap
nmap <tab> :call search('[A-Z]', 'W')<CR>
nmap <S-tab> :call search('[A-Z]', 'b')<CR>
set colorcolumn=0

```
press tab
press shift+tab

```
# Show git branch name
force_color_prompt=yes
color_prompt=yes
parse_git_branch() {
 git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
if [ "$color_prompt" = yes ]; then
 PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[01;31m\]$(parse_git_branch)\[\033[00m\]\$ '
else
 PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w$(parse_git_branch)\$ '
fi
unset color_prompt force_color_prompt
```


```
Vim spell
ftp://ftp.vim.org/pub/vim/runtime/spell/
Descargar el archivo en.utf-8.spl ponerlo en ~/.config/nvim/spell
Y
set spellfile=~/.config/nvim/spell/en.utf-8.dd
set spell
hi SpellBad guibg=#FF5733 ctermbg=30

```
