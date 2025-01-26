# Few-Steps-Terminal-Setup
🚀 A one-liner to install Starship, the blazing-fast, infinitely customizable shell prompt, using Snap.
# Starship Cross-Shell Prompt Installer 🚀

A quick guide to install and configure [Starship](https://starship.rs/), the minimal, blazing-fast shell prompt, on **Linux** and **macOS**.

## **Installation Methods**
sudo apt update
sudo apt install snapd


sudo snap install snap-store (optional)



### **1. Snap (Linux Only)**
```bash
sudo snap install starship --edge
```

### **2. Homebrew (macOS/Linux)**
```bash
brew install starship
```

### **3. Build from Source (Rust/Cargo)**
1. Install Rust:
   ```bash
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```
2. Install Starship:
   ```bash
   cargo install starship --locked
   ```

---

## **Configuration**

### **1. Initialize Starship**
Add to your shell’s config file:
- **Bash**: `~/.bashrc`
  ```bash
  eval "$(starship init bash)"
  ```
- **Zsh**: `~/.zshrc`
  ```zsh
  eval "$(starship init zsh)"
  ```
- **Fish**: `~/.config/fish/config.fish`
  ```fish
  starship init fish | source
  ```


---

## **Troubleshooting**
- **Icons Not Showing?**  
  Install a [Nerd Font](https://www.nerdfonts.com/) and configure your terminal.
- **Config Not Loading?**  
  Verify your shell’s config file is sourced (e.g., `source ~/.bashrc`).
- **Wayland/X11 Issues?**  
  Check session type:
  ```bash
  echo $XDG_SESSION_TYPE
  ```

---

## **Uninstall**
- **Snap**:
  ```bash
  sudo snap remove starship
  ```
- **Homebrew**:
  ```bash
  brew uninstall starship
  ```
- **Cargo**:
  ```bash
  cargo uninstall starship
  ```

---

## **References**
- [Official Docs](https://starship.rs/config/)
- [Preset Gallery](https://starship.rs/presets/)

---

🌟 **Enjoy your shiny new prompt!**  
```

---

This `README.md` is clean, platform-agnostic, and ready for GitHub. Customize it further with badges or additional details! 🎉
