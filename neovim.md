# Neovim

## Installation

Installation using flatpak
```bash
$ flatpak install flathub io.neovim.nvim
$ flatpak run io.neovim.nvim
```

Add the alias on `~/.bashrc` to run the flatpak with `nvim`
```bash
alias nvim="flatpak run io.neovim.nvim"
```

Reload the shell configuration
```bash
source ~/.bashrc
```

**Important:** Note that Flatpak'ed Neovim will look for `init.vim` in `~/.var/app/io.neovim.nvim/config/nvim` instead of `~/.config/nvim`.

## LazyVim

Install it in the flatpak config directory
```bash
git clone https://github.com/LazyVim/starter ~/.var/app/io.neovim.nvim/config/nvim
```

Remove the .git folder so I can push my configs to my own repo
```bash
rm -rf ~/.var/app/io.neovim.nvim/config/nvim/.git
```

Install repgrep to enable grep
```bash
$ sudo apt install ripgrep
```

## Configuration

Installing Firacode on debian
```bash
sudo apt install fonts-firacode
```

- Download Meslo on: https://www.nerdfonts.com/font-downloads
- Install:
  - MesloLGS Nerd Font Regular
  - MesloLGS Nerd Font Bold
  - MesloLGS Nerd Font italic
  - MesloLGS Nerd Font Bold italic
