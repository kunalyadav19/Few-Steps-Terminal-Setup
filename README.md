# Few-Steps-Terminal-Setup
🚀 A one-liner to install Starship, the blazing-fast, infinitely customizable shell prompt, using Snap.
# Starship Cross-Shell Prompt Installer 🚀

A quick guide to install and configure [Starship](https://starship.rs/), the minimal, blazing-fast shell prompt, on **Linux** and **macOS**.

## **Installation Methods**
sudo apt update

### **1. Install Starship  (Linux Only)**
```bash
sudo apt install snapd
sudo snap install snap-store (optional)
```
### **2. curl (Curl/Linux)** Fastest Way
```bash
curl -sS https://starship.rs/install.sh | sh
```
```bash
sudo snap install starship --edge
```

### **3. Homebrew (macOS/Linux)**
```bash
brew install starship
```

### **4. Generate the gruvbox-rainbow Preset or  (Any preset: https://starship.rs/presets/)**
** Easy to Install : Preset ***

```bash
curl -sS https://starship.rs/install.sh | sh
```

## **5 Verify the Configuration**
 Configuration:
Open the starship.toml file to ensure the preset has been applied:

```bash
cat ~/.config/starship.toml ```
## You should see a configuration that corresponds to the gruvbox-rainbow theme. ```

## **6 Set Up Starship in Your Shell**

To ensure Starship is loaded every time you open a terminal, add the following line to your shell's configuration file (e.g., .bashrc, .zshrc, or .bash_profile):

```bash
eval "$(starship init bash)"  # For Bash
eval "$(starship init zsh)"   # For Zsh
eval "$(starship init fish)"  # For Fish ```
Replace bash, zsh, or fish with your shell of choice.

Reload Your Shell:
After updating your shell configuration file, reload it to apply the changes:

```bash
source ~/.bashrc  # For Bash
source ~/.zshrc   # For Zsh
source ~/.config/fish/config.fish  # For Fish
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
