vimrc
=====

Yiyo's vimrc


Quick start
-----------

```
//Switch to neovim
//Install neovim with newest stable version

AppImage ("universal" Linux package)
The Releases page provides an AppImage that runs on most Linux systems. No installation is needed, just download nvim.appimage and run it. (It might not work if your Linux distribution is more than 4 years old.)

curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
chmod u+x nvim.appimage
./nvim.appimage
To expose nvim globally:

mkdir -p /opt/nvim
mv nvim.appimage /opt/nvim/nvim
And the following line to ~/.bashrc:

export PATH="$PATH:/opt/nvim/"

sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'

//create init.vim if it not exist
touch .config/nvim/init.vim

//add following in .config/nvim/init.vim
set runtimepath^=~/.vim runtimepath+=~/.vim/after
let &packpath = &runtimepath
source ~/.vimrc

git clone https://github.com/CYIYO/vimrc.git ~/vimrc
//if .vimrc and .vim exist, remove it first and do the following cmd
ln -s ~/vimrc/.vimrc ~/.vimrc
ln -s ~/vimrc/.vim ~/.vim

//instal vim-plug
curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
In vim execute :PlugInstall
```

NOTE
----------
tmux color issue:
```
add  "set -g default-terminal "xterm""  to ~/.tmux.conf 
```
Other Plugin needed:
```
sudo apt install cscope
sudo apt install universal-ctags
```
nerd font download:
```
https://github.com/Karmenzind/monaco-nerd-fonts
```



