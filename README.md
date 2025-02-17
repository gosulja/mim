# mim
My own personal minimal Neovim configuration for C/C++, Python and Lua development.

![2025-02-13_20-27](https://github.com/user-attachments/assets/262b7867-6952-4677-89c0-b23f85e66832)


# Requirements
* **Packer**
* **unzip**
* **clang** or **llvm**

# Installation
If you haven't installed **Packer**, you can easily do so by doing this:
```bash
$ git clone --depth 1 https://github.com/wbthomason/packer.nvim && ~/.local/share/nvim/site/pack/packer/start/packer.nvim
```

After **Packer** is installed, clone this repo and move the `init.lua` file to `~/.config/nvim/`
```bash
$ git clone --depth 1 https://github.com/gosulja/mim.git mim && mv ./mim/config/init.lua ~/.config/nvim/init.lua
```

When that's done, open Neovim.
```bash
$ nvim
```

Sync packer.
```bash
:PackerSync
```

If the language servers don't install automatically, install them:
```bash
:MasonInstall clangd pyright lua-language-server
```

Done!

# Changing Theme
If you'd like to change the theme of the config, simply call `use '<THEME>'` in the packer startup function, which starts on `line 3`.
For example, `use 'folke/tokyonight.nvim'` is the default theme being used, go to that line and replace it with your theme of choice.
After that, just make sure to setup the theme, like on `line 44`.
