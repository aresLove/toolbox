# i3 Window Manager

## 常用快捷键
$mod一般为Alt或Win键，初次启动i3时可进行设置。
* $mod + enter: opens a new terminal
* $mod + d: open application launcher (dmenu)
* $mod + shift + q: kill a window
* $mod + shift + e: exit i3
* $mod + shift + c: reload i3 configuration
* $mod + number: switch to another work space
* $mod + shift + number: move a window to another work space
* $mod + e: default container layout
* $mod + w: tabbed container layout
* $mod + f: toggle fullscreen
* $mod + shift + space: toggle floating
* $mod + mouse left button: drag floating

## 配置文件的路径

* /etc/i3/config
* ~/.i3/config
* ~/.config/i3/config


```
# Start i3bar to display a workspace bar (plus the system information i3status
# finds out, if available)
bar {
        status_command i3status
}

bindsym $mod+End exec /bin/bash -c 'i3lock -i <(import -window root - | convert -blur -5x5 - png:-)'

exec --no-startup-id fcitx
exec --no-startup-id clipit
```
