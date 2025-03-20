### Using kickstart in termux

BASH script allows you to manually install packages for mason.

## how to
```
pkg install which
```
download script
```
chmod +x pkg-install-mason
```
# clangd for example
```
./pkg-install-mason clangd
```

Script is mostly from https://github.com/Amirulmuuminin/setup-mason-for-termux.
I just added a way to automatically install clangd, since it’s not a standalone package in Termux.
It comes with clang.
