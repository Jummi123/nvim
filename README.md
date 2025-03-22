Readme for kickstart https://github.com/nvim-lua/kickstart.nvim  
It has quite comprehensive documentation. You can use that if you get stuck.

# Using neovim in termux

### Install neovim
```
pkg install neovim
```
Clone repository to ~/.config/nvim
```
git clone https://github.com/Jummi123/nvim.git ~/.config/nvim
```
You can check if you have everything you need by using
```
:checkhealt
```
in neovim.
### Installing language servers manually
Mason cannot install language servers for termux so we have to do it manually.
```
pkg install which
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
chmod +x pkg-install-mason
```
### Install Clangd for example
```
./pkg-install-mason clangd
```

