# [dot] files config

# Installation

### Clone

```
git clone git@github.com:HadesD/dotfiles.git ~/dotfiles && \
cd ~/dotfiles && \
git submodule update --init --recursive
```

### Vim

- Ubuntu

```bash
sudo apt-get install vim-gui-common vim-runtime clang1 clang-3.8-dev
```

- Symlink
```
ln -s ~/dotfiles/.vim ~/.vim && \
ln -s ~/.vim/.vimrc ~/.vimrc
```

_**Install YouCompleteMe**_
```bash
cd ~/.vim/bundle/YouCompleteMe && \
./install.py --all
```

_**Install VimProc**_
```
vi
:VimProcInstall
```
_or_
```
cd ~/.vim/bundle/vimproc.vim && make
```

### Tmux

- Symlink

```
ln -s ~/dotfiles/.tmux ~/.tmux && \
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf
```

### ZSH

- ZSH_CUSTOM

```
sed -i -e "1i export ZSH_CUSTOM=\$HOME/dotfiles/zshcustom" ~/.zshrc
```
