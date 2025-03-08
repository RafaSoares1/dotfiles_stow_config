# Dotfiles Management with Stow

This repository contains my configuration files (dotfiles) for various applications, managed using GNU Stow for easy symlink management.

## 📥 Installation on a New Machine

To use these dotfiles on another computer, follow these steps:

### 1️⃣ Install Required Packages
Ensure you have **Git** and **GNU Stow** installed:

#### Debian/Ubuntu:
```bash
sudo apt update && sudo apt install git stow -y
```

### 2️⃣ Clone the Repository
Clone this dotfiles repository to your home directory:

```bash
git clone <repo-url> ~/dotfiles
cd ~/dotfiles
```

### 3️⃣ Stow the Configurations
Run `stow` to create symlinks for the desired configurations:

```bash
stow zsh
stow tmux
stow lazygit
stow lazydocker
stow ranger
stow atuin
stow zoxide
```

**This will symlink the configuration files from `~/dotfiles/<package>` to `~/.<config_file>`.**

### ✅ Done!
Your dotfiles are now set up and easily manageable across different machines!
