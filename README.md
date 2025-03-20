readme for kickstart https://github.com/nvim-lua/kickstart.nvim

### Using kickstart in termux

BASH script allows you to manually install packages for mason.

# Install neovim
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
# Installing pakcages to mason
Mason cannot install language servers for termux so we have to do it manually.
```
pkg install which
```
# Download script

# Make executable
```
chmod +x pkg-install-mason
```
# Install Clangd for example
```
./pkg-install-mason clangd
```

Script is mostly from https://github.com/Amirulmuuminin/setup-mason-for-termux.
I just added a way to automatically install clangd, since it’s not a standalone package in Termux.
It comes with clang.
