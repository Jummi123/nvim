Readme for kickstart https://github.com/nvim-lua/kickstart.nvim  
It has quite comprehensive documentation. You can use that if you get stuck.

Script that is used here also installs: which, make, python, lua, ninja, rustup (so we can isntall asm-lsp), nodejs (for bash-language-server), stylua, clang (includes clangd).
# Using neovim in termux
Update package list
```
pkg update && pkg upgrade -y
```
### Install neovim
Get git first:)
```
pkg install git
```
```
pkg install neovim
```
Clone repository to ~/.config/nvim
```
git clone https://github.com/Jummi123/nvim.git ~/.config/nvim
cd ~/.config/nvim
```
Now run autoInstall if you are using my clone.
```
chmod +x autoInstall.sh
./autoInstall.sh
```
start neovim and after it does its thing, close it and done.  
It should now be working:)
### Installing language servers manually
Mason cannot install all language servers for termux so we have to do it manually.  
```
pkg install wget
```
### Download script
If you just want to install clangd, lua-language-server, stylua, etc...  
Then you can just use this script without cloning whole repo. 
```
wget https://raw.githubusercontent.com/Jummi123/nvim/refs/heads/master/pkg-install-mason
```

### Make executable
```
chmod +x lsp-install-mason
```
### Install Clangd for example
```
./pkg-install-mason clangd
```

Idea for this script came from https://github.com/Amirulmuuminin/setup-mason-for-termux
:)
