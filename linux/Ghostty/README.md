# Ghostty Terminal - Ubuntu Complete Configuration
font-family = "Maple Mono NF CN"
font-size = 15
font-thicken = true
adjust-cell-height = 6

theme = Kanagawa Wave

background-opacity = 0.85
background-blur = true

window-decoration = true
window-padding-x = 14
window-padding-y = 10
window-save-state = never
window-width = 80
window-height = 24
window-theme = auto

cursor-style = bar
cursor-style-blink = true
mouse-hide-while-typing = true
copy-on-select = clipboard

quick-terminal-position = top
quick-terminal-screen = mouse
quick-terminal-autohide = true
quick-terminal-animation-duration = 0.15

confirm-close-surface = false
clipboard-paste-protection = true
clipboard-paste-bracketed-safe = true

shell-integration = detect
shell-integration-features = cursor,sudo,no-title,ssh-env,ssh-terminfo,path

scrollback-limit = 100000

keybind = ctrl+shift+t=new_tab
keybind = ctrl+shift+left=previous_tab
keybind = ctrl+shift+right=next_tab
keybind = ctrl+shift+w=close_surface

keybind = ctrl+shift+d=new_split:right
keybind = ctrl+alt+d=new_split:down
keybind = ctrl+alt+left=goto_split:left
keybind = ctrl+alt+right=goto_split:right
keybind = ctrl+alt+up=goto_split:top
keybind = ctrl+alt+down=goto_split:bottom
keybind = ctrl+shift+e=equalize_splits
keybind = ctrl+shift+f=toggle_split_zoom

keybind = ctrl+plus=increase_font_size:1
keybind = ctrl+minus=decrease_font_size:1
keybind = ctrl+zero=reset_font_size

keybind = global:ctrl+grave_accent=toggle_quick_terminal

keybind = ctrl+shift+comma=reload_config
