# ⚡ Neon Force Updater v1.1.0

Single-click **FORCE** updater for all Linux distros — Discover-grade updates, but **nothing is normal, everything is forced, and ONE password prompt covers the whole run**.

**What's new in v1.1.0**
- 🔐 Single-auth runner — all 20 steps run inside one `pkexec` script, approve once
- ✔ No more FAILs — corrected apt flags (`update`/`autoclean` take no `-y`), benign "nothing to do" exits counted SUCCESS
- 📦 Snap/Flatpak file visibility — package lists BEFORE + AFTER (`snap list`, `snap changes`, per-app Flatpak table)
- 🪟 Frameless window with working left-side `— ▢ ✕` buttons (minimize/maximize/close click-tested on GNOME X11)
- 🧹 Overlap-free title + terminal layout

**Highlights**
- ⚡ One-click `FORCE UPDATE ALL`: APT + Snap + Flatpak + Firmware
- 🎯 Individual force buttons: APT / SNAP / FLATPAK / FIRMWARE
- 🌃 Dark neon luminous GUI (cyan/magenta/lime)
- ▣ Small live terminal — every step streams so you always see what's happening
- 🐧 Auto-detect: apt-get, dnf, pacman, zypper, snap, flatpak, fwupdmgr (ParrotSec latest ready)
- 📦 Portable AppImage — ~5.8 MB, no install

**Forced operations**
- `apt-get update`, `dpkg --configure -a --force-all`
- `install -f / dist-upgrade / full-upgrade / upgrade` with `--force-overwrite --force-confnew --force-conflicts --allow-downgrades --allow-remove-essential --allow-change-held-packages -y`
- `autoremove`, `autoclean`, `clean`
- `snap refresh` (+ before/after lists), `flatpak update --system/--user -y`, `flatpak repair`, `flatpak uninstall --unused -y`
- `fwupdmgr refresh --force`, `fwupdmgr update -y`

**Install & run**
```bash
chmod +x Neon-Force-Updater-1.1.0-x86_64.AppImage
./Neon-Force-Updater-1.1.0-x86_64.AppImage
```

**Verify**
- Size: 5982712 bytes (5.8M)
- SHA256: `17b0d54cb2c9c73ad3582946810846e95e301af415ed1004836e2cfaa633b183`

**Built from**
- Rust + eframe/egui 0.32, `neon-force-updater` v1.1.0
- Icon: neon lightning PNG + .desktop entry bundled in the AppImage
