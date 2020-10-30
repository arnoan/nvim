# VSCodium & Neovim

Reference:
[https://www.chrisatmachine.com/Neovim/22-vscodium-neovim/](Blog)
[https://github.com/ChristianChiarulli/nvim](Github)

## Installation

### Install Neovim (0.5)
### Install VSCodium

### Add the following to `product.json` to enable VSCode extensions:
(Path: ‎⁨macOS Mojave⁩ ▸ ⁨Applications⁩ ▸ ⁨VSCodium⁩ ▸ ⁨Contents⁩ ▸ ⁨Resources⁩ ▸ ⁨app⁩)

```json
"extensionsGallery": {
    "serviceUrl": "https://marketplace.visualstudio.com/_apis/public/gallery",
    "itemUrl": "https://marketplace.visualstudio.com/items"
}
```

### Install Extensions
- Neovim
- Whichkey
- Python

- Cobalt2 Theme
- Gitlens
- Remote - SSH
- AuzureML

### Adjust configuration files:
General/which-key settings: settings.json
Keybindings: keybindings.json
Neovim settings: vscodium_init.vim

Acess from VSCodium via Command Palette.
Point NeoVim extension to init.vim path.
Default: ```"$HOME/.config/nvim/vscodium_init.vim"```
