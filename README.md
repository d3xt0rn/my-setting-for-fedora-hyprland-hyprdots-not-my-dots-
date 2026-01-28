# Fedora Hyprland – My Settings (Not My Dots)

Personal Hyprland configuration based on **fedora-hyprland-hyprdots**, modified and adapted for my own workflow.

> ⚠️ This is **NOT** a plug-and-play setup.  
> You are expected to understand Hyprland and tweak configs for your system.

---

## 📸 Screenshot

![Desktop](https://github.com/user-attachments/assets/7f622d5e-3c80-49ab-b8b1-97c3c8710432)

> Screenshot from my current Hyprland setup

---

## ✨ About

This repository contains **my personal configuration** for:

- Hyprland
- Waybar
- Fastfetch
- CAVA

The base configuration was taken from:  
https://github.com/Senshi111/fedora-hyprland-hyprdots

Then modified, cleaned up and adapted for my daily usage.

---

## 🧩 Components

| Component | Description |
|---------|-------------|
| WM      | Hyprland    |
| Bar     | Waybar      |
| Fetch   | Fastfetch   |
| Audio   | CAVA        |
| Shell   | zsh         |
| Display | Wayland     |
| OS      | Fedora      |

---

## ⌨️ Keybindings (Main)

**Main modifier:** `SUPER`

### 🪟 Windows / Session

SUPER + Q              → Close focused window  
ALT   + F4             → Close focused window  
SUPER + Delete         → Exit Hyprland session  
SUPER + W              → Toggle floating mode  
ALT   + Enter          → Toggle fullscreen  
SUPER + L              → Lock screen  
SUPER + Backspace      → Logout menu  
CTRL  + ALT + W        → Restart Waybar  
SUPER + SPACE          → Switch keyboard layout  

---

### 🚀 Applications

SUPER + T              → Terminal (kitty)  
SUPER + E              → File manager (nautilus)  
SUPER + C              → Code editor (VS Code)  
SUPER + F              → Browser (Firefox)  
SUPER + A              → App launcher (rofi)  
SUPER + TAB            → Window switcher  

---

### 🧭 Workspaces

SUPER + 1..9           → Switch workspace  
SUPER + SHIFT + 1..9   → Move window to workspace  
SUPER + CTRL + ←/→     → Previous / Next workspace  
SUPER + Mouse Wheel    → Scroll workspaces  

---

### 🔊 Media / System

XF86AudioRaiseVolume   → Volume up  
XF86AudioLowerVolume   → Volume down  
XF86AudioMute          → Toggle mute  
XF86AudioPlay          → Play / Pause  
XF86MonBrightnessUp    → Brightness up  
XF86MonBrightnessDown  → Brightness down  

---

## 🔐 SSH Shortcut (Optional)

An **optional SSH keybind** is included in the config.

Example:

bind = SUPER+CTRL, S, exec, kitty -e ssh user@host

### ⚠️ Disabled by default

To enable it:

1. Open `~/.config/hypr/keybindings.conf`
2. Edit the SSH line:
   - replace `user@host`
   - or remove it completely if not needed

This shortcut is **optional** and safe to remove.

---

## 📥 Installation

Make sure you already have  
https://github.com/Senshi111/fedora-hyprland-hyprdots installed.

---

### 🔹 Clone repository

git clone https://github.com/d3xt0rn/my-setting-for-fedora-hyprland-hyprdots-not-my-dots-
cd my-setting-for-fedora-hyprland-hyprdots-not-my-dots-

---

### 🔹 Backup existing configs (recommended)

mkdir -p ~/.config-backup  
cp -r ~/.config/fastfetch ~/.config-backup/ 2>/dev/null  
cp -r ~/.config/waybar   ~/.config-backup/ 2>/dev/null  
cp -r ~/.config/hypr     ~/.config-backup/ 2>/dev/null  
cp -r ~/.config/cava     ~/.config-backup/ 2>/dev/null  

---

### 🔹 Install Fastfetch

mkdir -p ~/.config/fastfetch  
cp -r fastfetch/* ~/.config/fastfetch/

---

### 🔹 Install CAVA

mkdir -p ~/.config/cava  
cp -r cava/* ~/.config/cava/

---

### 🔹 Install Waybar

mkdir -p ~/.config/waybar  
cp -r waybar/* ~/.config/waybar/

---

### 🔹 Install Hyprland

mkdir -p ~/.config/hypr  
cp -r hyprland/* ~/.config/hypr/

---

### 🔹 Reload Hyprland

hyprctl reload  

Or simply **log out and log back in**.

---

## 🧠 Notes

- Tested on **Fedora**
- Wayland only
- Fonts, icons and wallpapers are **not included**
- NVIDIA users may require additional flags

---

## 🧾 License

MIT

---

## 🤝 Credits

Original project:

- **Senshi111** – fedora-hyprland-hyprdots

Configs modified and maintained by **d3xt0rn**
