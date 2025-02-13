# mim
My own personal minimal Neovim configuration for C/C++, Python and Lua development.

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
$ git clone --depth 1 https://github.com/gosulja/mim.git && mv ./mim/init.lua ~/.config/nvim/init.lua
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
