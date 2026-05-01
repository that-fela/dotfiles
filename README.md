# dotfiles

Simple Linux dotfiles managed with GNU Stow.

## install

```bash 
git clone https://github.com/that-fela/dotfiles ~/.dotfiles
cd ~/.dotfiles
```

install deps:

```bash
sudo apt update
sudo apt install zsh tmux stow
```

Install [Neovim](https://github.com/neovim/neovim) (11.x):

(optional) set zsh as default shell:

```bash
chsh -s $(which zsh)
```

## usage

stow all packages (recursive, handles oh-my-zsh):

```bash
stow -R */
```

## notes

* run from repo root
* each folder is a package
* files get symlinked into ~
