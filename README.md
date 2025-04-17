# Installation Instructions

### Linux

Backup your original tmux config (if exists).

```
mv ~/.config/tmux/ ~/.config/tmux.bak
mv ~/.tmux.conf ~/.tmux.conf.bak
```

Remove your old tmux config.

```
rm -rf ~/.config/tmux ~/.tmux.conf
```

Git clone the repository and install the config.

```
git clone --depth 1 https://github.com/NightSling/dotfiles-tmux.git ~/.config/tmux
ln -s ~/.config/tmux/tmux.conf ~/.tmux.conf
```

Install the plugin manager.

```
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

Install the catpuccin theme

```
mkdir -p ~/.config/tmux/plugins/catppuccin
git clone -b v2.1.3 https://github.com/catppuccin/tmux.git ~/.config/tmux/plugins/catppuccin/tmux
```

Install the plugins after starting `tmux` with `Ctrl+A Shift+I`.
