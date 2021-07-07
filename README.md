# My dotfiles currently used on my WSL2 setup (Work in Progress)

Info: Dotfiles are synced with GNU Stow [How To](https://www.youtube.com/watch?v=CFzEuBGPPPg&t=2053s&ab_channel=DevInsideYou)
1. Clone and cd into this repo
2. Run `stow -vSt ~ *` to unstow everything or pick the configuration explicitly e.g. `stow -vSt ~ zsh`

In order to stow configuration files 
1. Create correct folder structure in package folder within the .dotfiles directory
2. Run `stow --adopt -vt ~ */`

## Prepare WSL2

- Install Windows Terminal
- Install a nerd font and configure it as the default font family for the distro (Ubuntu 20.04). I am currently using 'Meslo LGMDZ NF'

## Configure Zsh

- Install Zsh with oh-my-zsh
- Install powerlevel10k
- Install zsh-plugins `zsh-syntax-highlighting`,`zsh-autosuggestions`,`zsh-completions`,`fzf-tab`

Tools:

- stow
- fd (fd-find)
- bat (batcat)
- ripgrep
- fzf
- fasd
- tree
- build-essential
- rust
- exa (`cargo install exa`)
- dust (`cargo install du-dust`)
- net-tools
- neovim 0.5 (with LunarVim configuration)
- jq
- node
- npm
- python3
- java 

Links:

- https://medium.com/better-programming/boost-your-command-line-productivity-with-fuzzy-finder-985aa162ba5d
- https://chaosstate.com/posts/vim-navigate-like-a-wizard/

ripgrep currently has a conflict with bat. Try to install like below<br>
`$ apt-get download ripgrep`<br>
`$ sudo dpkg --force-overwrite -i ripgrep*.deb`<br>
