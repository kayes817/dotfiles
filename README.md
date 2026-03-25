# Dotfiles

This directory is organized for GNU Stow.

## Packages

- `shell`: installs `.zshrc`
- `alacritty`: installs `~/.config/alacritty/alacritty.toml`
- `hypr`: installs `~/.config/hypr/hyprland.conf`
- `waybar`: installs `~/.config/waybar/`
- `bin`: installs helper scripts into `~/.local/bin/`

## Usage

From this directory:

```bash
stow -t "$HOME" shell alacritty hypr waybar bin
```

To refresh links after edits, run the same command again.
