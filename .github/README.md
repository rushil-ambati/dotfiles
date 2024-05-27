# Dotfiles

## Installation

```sh
git clone --bare https://github.com/rushil-ambati/dotfiles.git $HOME/.config/dotfiles
# backup or remove existing files
git --git-dir=$HOME/.config/dotfiles --work-tree=$HOME config checkout
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
