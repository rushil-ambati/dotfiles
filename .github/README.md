# Dotfiles

## Installation

### Requirements

- [`zsh + oh-my-zsh`](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)
- [`powerlevel10k`](https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#oh-my-zsh)
- [`zsh-autosuggestions`](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#oh-my-zsh)
- [`zsh-syntax-highlighting`](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#oh-my-zsh)
- [`you-should-use`](https://github.com/MichaelAquilina/zsh-you-should-use?tab=readme-ov-file#installation)
- [`fzf`](https://github.com/junegunn/fzf?tab=readme-ov-file#installation) + [`fzf-tab`](https://github.com/Aloxaf/fzf-tab?tab=readme-ov-file#oh-my-zsh)
- [`atuin`](https://docs.atuin.sh/guide/installation/)
- [`bat`](https://github.com/sharkdp/bat?tab=readme-ov-file#installation)
- [`eza`](https://github.com/eza-community/eza/blob/main/INSTALL.md#installation)
- [`neovim`](https://github.com/neovim/neovim/blob/master/INSTALL.md) ([`lazy.nvim`](https://github.com/folke/lazy.nvim?tab=readme-ov-file#-installation))
- [`tmux`](https://github.com/tmux/tmux/wiki/Installing#installing-tmux) + [`tpm`](https://github.com/tmux-plugins/tpm?tab=readme-ov-file#installation) (catppuccin included)
- `notify-send` on Linux

> Note: Be sure to back up all existing dotfiles before proceeding.

```sh
git clone --bare https://github.com/rushil-ambati/dotfiles.git $HOME/.config/dotfiles
git --git-dir=$HOME/.config/dotfiles --work-tree=$HOME checkout
exec zsh
config config --local status.showUntrackedFiles no
```

## Pulling changes

```sh
config pull
```

## Pushing changes

```sh
config status
config add .zshrc
config commit -m "Add zshrc"
config push
```
