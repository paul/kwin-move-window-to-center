# Installation Instructions
## Graphical Installation
Navigate to `System Settings > Window Management > KWin Scripts` and:
* Either click on the `Install from File...` button and browse for the downloaded script,
* or click on the `Get New Scripts...` button and search for the script online through the `Get Hot New Stuff` dialog.

## Console Installation
```shell
kpackagetool5 --install /path/to/movewindowtocenter.kwinscript
```

## Restart KWin
Before being able to use this script it's required to restart KWin.
* Either restart KWin via console
  ```shell
  # for X11
  killall kwin_x11 && kwin_x11 &
  
  # for Wayland
  killall kwin_wayland && kwin_wayland &
  ```
* or just restart the system

# Uninstallation Instructions
If you installed the script through the `Get Hot New Stuff` dialog, you should uninstall it through the same dialog, otherwise the following command will do:

```shell
kpackagetool5 --type KWin/Script --remove movewindowtocenter
```
