# Hyprland on Fedora
This is my Hyprland configs on Fedora Workstation. Feel free to edit and use it!!

## Preview
**The main desktop**

![Main Window](screenshots/)

**Terminal**

![Kitty and Alacritty](screenshots/)

**Running an Apps**

![Firefox](screenshots/)

## What's Inside?

- **Window Manager:** [Hyprland](https://hyprland.org/) - Our favorite wayland compositor !!
- **Bar:** [Waybar](https://github.com/Alexays/Waybar) - Simple, clean and very customizeable
- **Launcher:** [Rofi](https://github.com/davarotium/rofi) - Easy and fast app launcher
- **Notifications:** [SwayNC](https://github.com/ErikReider/SwayNotificationCenter) - Beautiful and simple notification center
- **Wallpaper:** [Hyprpaper](https://github.com/hyprwm/hyprpaper) + [SWWW](https://github.com/LGFae/swww) for smooth transition
- **Lock Screen:** [Hyprlock](https://) better than swaylock i guess
- **Terminal:** [Kitty](https://sw.kovidgoya1.net/kitty/) (main) and [Alacritty](https://alacritty.org/) (backup)
- **Shell:** [Zsh](https://www.zsh.org/) with [Starship](https://starship.rs/) prompt
- **Text Editor:** [Neovim](https://neovim.io/) A very powerful text editor

## Installation Guide

### You'll need these packages

```bash
# the essentials
hyprland waybar rofi-wayland swaync swaylock hyprpaper hypridle swww

# terminal stuff
kitty alacritty zsh starship

# other stuff i use
polkit-gnome networkmanager pavucontrol neovim fastfetch btop eza
```

### Using Stow (the easy method)

I use GNU Stow to manage everything. If you don't have it, just `sudo dnf install stow` (if u're using Fedora)

```bash
git clone https://github.com/yourusername/dotfiles.git ~dotfiles
cd ~/dotfiles

# symlink everything at once
stow alacritty hyprland kittyterminal nvim rofi starship hyprlock swaync waybar zsh

# or just what you need
stow hyprland waybar hyprlock
```

### Manual way

if you don't want to use stow, just copy these configs:

```bash git clone https://github.com/yourusername/dotfiles.git ~/dotfiles

cp -r ~/dotfiles/hyprland/.config/hypr ~/.config/
cp -r ~/dotfiles/waybar/.config/waybar ~/.config/
# and so on ... you get the idea

cp ~/dotfiles/zsh/.zshrc ~/
```

## Keybindings

All my keybinds are in `hyprland/.config/hypr/modules/binds.conf` - customize those keybinds all by yourself until it suits you

