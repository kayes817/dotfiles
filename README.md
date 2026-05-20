# Dotfiles

This directory is organized for GNU Stow.

## Packages

- `shell`: installs `.zshrc`
- `alacritty`: installs `~/.config/alacritty/alacritty.toml`
- `hypr`: installs `~/.config/hypr/hyprland.conf`
- `waybar`: installs `~/.config/waybar/`
- `bin`: installs helper scripts into `~/.local/bin/`
- `gtk`: installs GTK settings including icon theme

## Usage

From this directory:

```bash
stow -t "$HOME" shell alacritty hypr waybar bin gtk
```

To refresh links after edits, run the same command again.

## Wallpaper Helper

`bin/.local/bin/wallpaperctl` looks for wallpapers in:

- `~/Wallpapers/`
- `~/Pictures/Wallpapers/`
- `~/.local/share/wallpapers/`

Apply the current wallpaper and regenerate Waybar/Rofi colors:

```bash
~/.local/bin/wallpaperctl apply
```
