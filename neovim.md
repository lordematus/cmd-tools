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
