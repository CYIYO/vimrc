vimrc
=====

StevenTing's vimrc


Quick start
-----------

```
//Switch to neovim
//Install neovim with newest stable version

sudo add-apt-repository ppa:neovim-ppa/stable
sudo apt-get update
sudo apt-get install neovim

sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'

//create init.vim if it not exist
touch .config/nvim/init.vim

//add following in .config/nvim/init.vim
set runtimepath^=~/.vim runtimepath+=~/.vim/after
let &packpath = &runtimepath
source ~/.vimrc

git clone https://github.com/CYIYO/vimrc.git ~/vimrc
//if .vimrc and .vim exist, remove if first and do the following cmd
ln -s ~/vimrc/.vimrc ~/.vimrc
ln -s ~/vimrc/.vim ~/.vim

In vim execute :PlugInstall
```

NOTE
----------
nerd font download:
===
```
https://github.com/Karmenzind/monaco-nerd-fonts
```



