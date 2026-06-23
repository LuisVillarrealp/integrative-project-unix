# Part 1 — Custom Distro with Cubic

**Author:** Ariel Buitron (@AreloXD2)

## Base ISO
Linux Mint 22.3 Cinnamon 64-bit (Wilma)

## Modifications

### 1. Firefox → LibreWolf
LibreWolf is a privacy-focused browser with no telemetry and enhanced security by default. Firefox was removed and replaced to give users a more private browsing experience out of the box.

### 2. MPV (media player)
MPV is a lightweight open-source media player that supports more codecs than the default player. It runs efficiently on low-resource systems and is highly configurable via terminal.

### 3. Neovim + /etc/skel configuration
Neovim is a modern terminal-based IDE. The configuration was placed in `/etc/skel/.config/nvim/` so every new user gets Neovim pre-configured with line numbers, mouse support, and syntax highlighting automatically.

### 4. Default theme via gschema
A custom gschema override file was created to set the dark theme as default for all users. This ensures the customization is persistent and applies system-wide, not just for one user.