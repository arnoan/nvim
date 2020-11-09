# VSCodium & Neovim

References:  
[Blog](https://www.chrisatmachine.com/Neovim/22-vscodium-neovim/)  
[Video Demonstration](https://www.youtube.com/watch?v=g4dXZ0RQWdw)  
[Github](https://github.com/ChristianChiarulli/nvim)  


[Youtube VSCode Tutorial](https://www.youtube.com/watch?v=WPqXP_kLzpo)

## Installation

### Install Neovim (0.5)
### Install VSCode Insiders Edition

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

Configure Neovim Extenion
- Path to neovim 0.5 binary 
- Path to neovim configuration: `"$HOME/.config/nvim/neovim_vscode_init.vim"`

### Key remappings
The key remapping (CAPSLOCK -> ESC+CTRL) configuration files for karabiner (macOS) or autohotkey (Windows) are [in my .dotfiles repository](https://github.com/arnoan/.dotfiles/tree/vscode_neovim/.config). 

### To update this repo if VSCode settings change
- clone this repo
- delete contained .json settings (since they have different inode)
    - `cd nvim/vscode_config/`
    - `rm keybindings.json settings.json`
- create hard links again
    - `ln /Users/arno/Library/Application\ Support/Code\ -\ Insiders/User/keybindings.json . && ln /Users/arno/Library/Application\ Support/Code\ -\ Insiders/User/settings.json .`
- Now changes in VSCode settings are automatically reflected in repo folder
