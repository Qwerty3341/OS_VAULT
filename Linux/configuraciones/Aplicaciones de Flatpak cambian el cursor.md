# Verificar el tema del cursor
```bash
grep -i "Inherits\|Name" ~/.icons/default/index.theme 2>/dev/null
 
grep -i "Inherits\|Name" /usr/share/icons/default/index.theme 2>/dev/null
Inherits=Adwaita 
```

```bash
xfconf-query -c xsettings -p /Gtk/CursorThemeName -n -t string -s Adwaita

flatpak override --user --env=XCURSOR_THEME=Adwaita
flatpak override --user --env=XCURSOR_SIZE=43
```
