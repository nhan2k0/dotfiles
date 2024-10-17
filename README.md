# dotfiles
my arch linux dotfiles using pywal for color scheme (coming soon)

## spicetify
this scheme is designed to use with the "text" theme

paste the lines below into the `color.ini` file inside the theme folder and apply using `spicetify config color_scheme pywal`.
> [!NOTE]
> you will need xrdb for loading the generated xresources file!
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
