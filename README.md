Installation:

```
sudo apt-get install vim-gtk
```

1) clone
`````
git clone git@github.com:rivanenko/vim.git ~/.vim
`````
2) create symlink
````````````
ln -s  ~/.vim/.vimrc ~/.vimrc
````````````
3) add vundle
````````
git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle
````````
4) open gvim and enter:
``````````
:BundleInstall
``````````

If you have warnings:

1) `Unable to create Ubuntu Menu Proxy: Timeout was reached`

2) `Trying to remove a child that does not believe we are it is parent.`

add in `~/.bashrc` the lines and restart the terminal
``````
function gvim () { (/usr/bin/gvim -f "$@" &>/dev/null &) }
alias gvim='UBUNTU_MENUPROXY= gvim'
``````
