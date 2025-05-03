# Overview and installation
This is my custom config files for Arch based Hyprland setup using Nord theme. Before installation you need to install Arch with needed graphic drivers. Then clone this repository, manualy install all packages and copy config files to folders. 

Installation script will be released later.

# Needed packages
```
sudo pacman -S hyprland kitty dolphin dolphin-plugins code firefox rofi-wayland pavucontrol waybar chromium pulseaudio qt5ct qt6ct qt5-wayland qt6-wayland kvantum cliphist xdg-desktop-portal-hyprland archlinux-xdg-menu sddm xorg nwg-look ark nm-connection-editor libnotify dunst pipewire wireplumber hyprpolkitagent unzip playerctl uwsm

yay -S oh-my-posh hyprshot hyprcursors Nordzy-cursors Nordzy-hyprcursors wlogout
```

# Fonts
```
yay -S ttf-font-awesome ttf-cascadia-code-nerd ttf-jetbrains-mono-nerd
```

# SDDM
Enabling:
`systemctl enable sddm`

Creating autologin in SDDM:
Change in /usr/lib/sddm/sddm.conf.d/default.conf `Session=` to `Session=hyprland-uwsm` and `User=` to `User=USER_NAME`

# Folders and files to copy
Copy config files from repository to theese locations:
- ~/.themes
- ~/.config/dolphinrc
- ~/.config/gwenviewrc
- ~/.config/kdeglobals
- ~/.config/dunst/.
- ~/.config/oh-my-posh/.
- ~/.config/hypr/.
- ~/.config/wlogout/.
- ~/.config/waybar/.
- ~/.config/Kvantum/.
- ~/.config/kitty/.
- ~/.config/rofi/.
- ~/.bashrc
- /etc/bash.bashrc

# Changing themes and icons in dolphin
1. Nord theme folder: copy to /usr/share/themes
2. Nord icons folder: copy existing breeze folder from /usr/share/icons to the same folder with different name -> сopy icons to this folder replacing files -> add theme to ~/.config/kdeglobals

# Enabling oh-my-posh config 
*(it is already done in provided .bashrc and bash.bashrc files)*
```
echo "eval \"\$(oh-my-posh init bash --config ~/.config/oh-my-posh/nordtron.omp.json\"" >> ~/.bashrc
echo "eval \"\$(oh-my-posh init bash --config home/${username}/.config/oh-my-posh/nordtron-root.omp.json\"" >> /etc/bash.bashrc
```

# Screenshots


# Links
[Hyprland repository](https://github.com/hyprwm/Hyprland)

[Nord theme official site](https://www.nordtheme.com/)

[Nordic wallpapers](https://github.com/linuxdotexe/nordic-wallpapers)

[My custom script for clean Arch install](https://github.com/Krestomansy/clean-arch-install)
