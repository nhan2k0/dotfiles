# dotfiles
my arch linux dotfiles using pywal for color scheme (coming soon)

## how to install
> [!NOTE]
> yay (or other AUR helper) is required as we need some packages there

first, install the packages with this command
```
yay -S hyprland-bin kitty waybar swaync rofi-wayland waypaper ttf-iosevka-nerd brightnessctl pamixer \
polkit-kde-agent noto-fonts-emoji python-pywal16 python-haishoku \
starship hyprshot xdg-desktop-portal-hyprland-git hyprpicker \
gvfs udiskie hyprlock ranger wl-paste wl-clip-persist \
```

## spicetify
this scheme is designed to use with the "text" theme, which you can get from [here](https://github.com/spicetify/spicetify-themes)

paste the lines below into the `color.ini` file inside the theme folder and apply using `spicetify config color_scheme pywal`.
> [!NOTE]
> you will need xrdb for loading the generated xresources file!
> 
> plus, if you do not like having to play the music manually because the client restarts, enable devtools using `spicetify apply enable-devtools` and use the update command (a manual reload of the client is required but the stream should not be interrupted)
```
[pywal]
accent = ${xrdb:color5}
accent-active = ${xrdb:color5}
accent-inactive = ${xrdb:background}
banner = ${xrdb:background}
border-active = ${xrdb:color5}
border-inactive = ${xrdb:foreground}
banner = ${xrdb:color14}
highlight = ${xrdb:color8}
main = ${xrdb:background}
notification = {xrdb:color8}
notification-error = ${xrdb:color4}
subtext = ${xrdb:color14}
text = ${xrdb:foreground} 
header = ${xrdb:color14}
```
