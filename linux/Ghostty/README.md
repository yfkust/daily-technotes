# 🚀 Ghostty 终端配置：

## 🎨 Ghostty Terminal - Ubuntu Complete Configuration
**位置**：nano ~/.config/ghostty/config

```conf
# ============================================
# Ghostty Terminal - Ubuntu Complete Configuration
# ============================================

# --- 字体与排版 ---
font-family = "Maple Mono NF CN"
font-size = 15
font-thicken = true
adjust-cell-height = 6

# --- 主题与透明度 ---
theme = Kanagawa Wave
# 半透明
background-opacity = 0.85
background-blur = true

# --- 窗口与外观 ---
window-decoration = true
window-padding-x = 14
window-padding-y = 10
window-save-state = never
window-width = 80
window-height = 24
window-theme = auto

# --- 光标与鼠标 ---
cursor-style = bar
cursor-style-blink = true
mouse-hide-while-typing = true
copy-on-select = clipboard

# --- 下拉式快捷终端 (Quake-style) ---
quick-terminal-position = top
quick-terminal-screen = mouse
quick-terminal-autohide = true
quick-terminal-animation-duration = 0.15

# --- 关闭行为与安全 ---
confirm-close-surface = false
clipboard-paste-protection = true
clipboard-paste-bracketed-safe = true

# --- 外壳集成 ---
shell-integration = detect
shell-integration-features = cursor,sudo,no-title,ssh-env,ssh-terminfo,path

# --- 性能优化 (重要！原来的缓存设得太大了) ---
scrollback-limit = 100000

# ============================================
# --- 快捷键配置 ---
# ============================================

# 标签页管理 (Linux 下用 ctrl+shift)
keybind = ctrl+shift+t=new_tab
keybind = ctrl+shift+left=previous_tab
keybind = ctrl+shift+right=next_tab
keybind = ctrl+shift+w=close_surface

# 分屏管理
keybind = ctrl+shift+d=new_split:right
keybind = ctrl+alt+d=new_split:down
keybind = ctrl+alt+left=goto_split:left
keybind = ctrl+alt+right=goto_split:right
keybind = ctrl+alt+up=goto_split:top
keybind = ctrl+alt+down=goto_split:bottom
keybind = ctrl+shift+e=equalize_splits
keybind = ctrl+shift+f=toggle_split_zoom

# 字体大小调节
keybind = ctrl+plus=increase_font_size:1
keybind = ctrl+minus=decrease_font_size:1
keybind = ctrl+zero=reset_font_size

# 全局呼出快捷键 (按下 Ctrl + ` 键可以像游戏控制台一样滑出/隐藏终端)
keybind = global:ctrl+grave_accent=toggle_quick_terminal

# 重新加载配置
keybind = ctrl+shift+comma=reload_config
```
