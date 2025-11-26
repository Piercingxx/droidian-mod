# Linux‑Phone‑Mod

Debian‑based phone setup in one go.  
Installs essentials, applies Piercing‑Dots GNOME tweaks, and readies your device for the attempt at daily use.

---

## 📦 Features

- Works on Debian‑based GNOME mobile OS: Droidian (Phosh), Mobian (Phosh), Ubuntu Touch, PureOS
- Installs core apps and tooling: Neovim Nightly, Yazi (+ plugins), GNOME Tweaks, Mission Center
- Adds Flathub (FLOSS subset) and Homebrew, sets up fonts and shell environment
- Waydroid installation (apt or repo fallback), Proton VPN desktop, Tailscale (manual service install)
- Enables UFW with SSH rules and performs system cleanups/updates
- Applies Piercing‑Dots GNOME customizations and replaces `.bashrc` with the standard PiercingXX config
    - All the .scripts are fully functional as well.

---

## 🚀 Quick Start

```bash
sudo apt update && sudo apt install git -y
git clone https://github.com/PiercingXX/linux-phone-mod
cd linux-phone-mod
chmod -R u+x scripts/
./linux-phone-mod.sh
```

> Note: The full install can take a while (often hours) on mobile hardware.

---

## 🛠️ Usage

Run `./linux-phone-mod.sh` and follow the menu prompts.

Menu options:
- Install – Runs prerequisites, applies Piercing‑Dots (including GNOME customizations), installs apps, updates shell
- Reboot System – Reboots when you’re ready
- Exit – Quit without changes

The script will clone and use the Piercing‑Dots repo during setup, then clean up.

---

## 📱 Tested On

- Google Pixel 3a
  - Droidian (Phosh)
  - Ubuntu Touch
- Librem 5
  - PureOS
  - Mobian (Phosh)

> Active daily‑driver testing. Expect changes; mobile Linux platforms evolve quickly or stagnate and die.

---


## ⚙️ What Gets Installed (Highlights)

- Homebrew + Flathub (FLOSS subset) remotes
- Neovim Nightly, Lua 5.4, Python pip, ripgrep, chafa
- Yazi file manager with curated plugins and helpers
- Waydroid (via apt or repo.waydro.id)
- UFW configured (SSH allowed); Proton VPN desktop client
- Tailscale (manual install, systemd service enabled)
- Piercing‑Dots GNOME customizations and standard `.bashrc`

---

## 📄 License

MIT © PiercingXX  
See the LICENSE file for details.

---

## 🤝 Contributing

Fork, branch, and PR welcome.  
Keep scripts POSIX‑friendly and avoid hard‑coded paths.

---

## 📞 Support

No direct support provided. Please open an issue if something breaks.
