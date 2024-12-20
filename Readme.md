# Cloning the config

#### Linux
```bash
git clone https://github.com/danisaski/neodafer.git ~/.config/nvim
```

#### Windows
```powershell
git clone https://github.com/danisaski/neodafer.git %userprofile%\AppData\Local\nvim
```

<details> <summary>Manual installation</summary>

# Manual installation

## Deleting local config 

#### Linux
```bash
rm -rf ~/.local/share/nvim
rm -rf ~/.config/nvim
```

#### Windows
```powershell
rd /s /q %userprofile%\AppData\Local\nvim
rd /s /q %userprofile%\AppData\Local\nvim-data
```

<details> <summary>Click to expand misc. notes</summary>
  
## Installing lazy.nvim

#### Linux
```bash
git clone https://github.com/folke/lazy.nvim.git ~/.local/share/nvim/lazy/lazy.nvim
```

#### Windows
```powershell
git clone https://github.com/folke/lazy.nvim.git %userprofile%\AppData\Local\nvim\lazy\lazy.nvim
```

# Python Dependencies

### Install a Python language server, linter and formatter
```bash
pip install pyright ruff
```

# OS Dependencies

### Install ripgrep and fzf for telescope/fzf-lua

#### Linux
```bash
sudo apt install ripgrep fzf
```

#### Windows
```powershell
winget install BurntSushi.ripgrep.MSVC
```

### Personal notes
#### Set-url SSH
```bash
git remote set-url origin git@github.com:danisaski/neodafer
```
#### Extract neovim tar.gz
```bash
tar -xvzf nvim-linux64.tar.gz
```
#### mv appropiate location
```bash
sudo mv nvim-linux64 /usr/local/nvim
```
#### Add to .bashrc
```bash
export PATH="/usr/local/nvim/bin:$PATH"
source ~/code/python/venvs/denv/bin/activate
```

**TODO:** Debugger interface and config for RUST
ensure installed equivalent to debugpy. Reorder pluggins.lua. Autoinstall nodejs, etc.
