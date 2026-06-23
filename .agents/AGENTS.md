# 🌌 Antigravity Profile: Saeedul's System & Workspace Context

This file serves as a persistent context record for Antigravity (AGY). When executing in this workspace, AGY should read this file to understand the developer's hardware, past environment configurations, and preferences.

---

## 👤 Developer Profile
*   **Name**: Saeedul
*   **Aesthetic Preference**: Gruvbox (Matte Black / Dark themes), clean monospace styling.
*   **Command Terminal**: Ghostty (Primary), Alacritty (Backup).
*   **GitHub**: `saeedullah-dev`

---

## 💻 Hardware Configuration
*   **Host Machine**: Lenovo ThinkPad T490 (Product ID: `20QES53R00`)
*   **Processor**: Intel Core i5-8365U (Whiskey Lake Architecture)
*   **Integrated Graphics**: Intel UHD Graphics 620
*   **Keyboard**: AT Translated Set 2 Keyboard
*   **TrackPoint**: TPPS/2 Elan TrackPoint (Requires scroll-emulation setup)
*   **WWAN Mobile Modem**: Intel XMM 7360 / Fibocom L850-GL PCIe LTE Modem

---

## 🐧 Legacy Ubuntu Linux Environment
*   **OS**: Ubuntu 26.04 (GNOME, Snaps, and GDM3 purged for minimal console boot)
*   **Window Manager**: Sway WM (Tiling)
*   **Status Panel**: Waybar
*   **App Launcher**: Rofi-Wayland
*   **Input Setup**: Custom Python service (`trackpoint_space_scroll.py`) mapped to translate `Caps Lock` holds + TrackPoint movement into vertical and horizontal scrolling.
*   **Modem Configuration**: Utilized `mmcli` and `socat` commands to unlock modem clock frequencies (`at@nvm:fix_cat_fcclock.fcclock_mode=0`) and systemd sleep hooks (`iosm-resume`) to handle sleep wake cycles.

---

## 🍏 macOS Transition / Hackintosh Environment
*   **Target OS Version**: macOS Tahoe (macOS 16 - final version to support Intel processors)
*   **Bootloader**: OpenCore (RELEASE versions)
*   **SMBIOS Configuration**: Spoofed to `MacBookPro15,2` (native 8th Gen Whiskey Lake platform)
*   **Intel UHD 620 Framebuffer**: Device ID spoofed to Coffee Lake (`9B3E0000`) with framebuffer platform ID `0900A53E` and stolen memory set to 19MB.
*   **Wi-Fi / Bluetooth**: Driven via Intel OpenIntelWireless stack (`itlwm.kext`, `IntelBluetoothFirmware.kext`, `BlueToolFixup.kext`).
*   **Modem WWAN**: Unsupported under macOS (requires Wi-Fi or phone hotspot sharing).
*   **Tiling & Customization**:
    *   Window Manager: **AeroSpace** (using standard Sway-compatible HJKL binding profiles).
    *   Status Bar: **SketchyBar**.
    *   Launcher: **Raycast**.
    *   TrackPoint Mapping: Replaced Linux python helper with **Karabiner-Elements** rules (emulating scroll when Caps Lock is pressed).

---

## 🤖 Instructions for Antigravity (AGY)
When working with Saeedul in this repository:
1.  **Aesthetics**: Always default to modern, high-contrast dark modes or Gruvbox color values when designing HTML, CSS, or terminal UI configurations.
2.  **Keyboard Habit**: Keep in mind that Saeedul prefers tiling layouts. Keep the AeroSpace config (`aerospace.toml`) aligned with standard Sway shortcuts (`Alt` bindings for window movement, terminal launches, and killing containers).
3.  **TrackPoint Emulation**: Refer to the Karabiner rules or the local `trackpoint_space_scroll.py` script to understand input mappings if trackpoint adjustments are needed.
