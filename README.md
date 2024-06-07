# My Dotfiles

This directory contains my system dotfiles for my Debian (Kali) configuration

## Requirements

I really need to test this out, but I think the following things are required:

- Alacritty
- fzf
- JetBrainsMono Nerd Font
- Stow
- Tmux

## Installation of Requirements
```bash
# install alacritty
$ cargo install --locked alacritty

# install fzf
$ git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf install

# download, unzip, and install JetBrainsMono nerd font
$ wget -P ~/.local/share/fonts https://github.com/ryanoasis/nerd-fonts/releases/download/v3.2.1/JetBrainsMono.zip
$ cd ~/.local/share/fonts
$ unzip JetBrainsMono.zip
$ rm JetBrainsMono.zip
$ fc-cache -fv
```

## Usage
```
git clone <this_repo>
cd dotfiles
stow --adopt .
```
