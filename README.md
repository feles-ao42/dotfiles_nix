# Nix version dotfiles

## nix
https://nixos.org/download#nix-install-macos

```
sh <(curl -L https://nixos.org/nix/install)
```
## change shell

```
chsh -s $(which zsh)
```

## home-manager
https://nix-community.github.io/home-manager/index.html#sec-install-standalone

```
nix-channel --add https://github.com/nix-community/home-manager/archive/release-23.05.tar.gz home-manager
nix-channel --update
nix-shell '<home-manager>' -A install
```

```
rm ~/.config/home-manager/home.nix
ln home-manager/home.nix ~/.config/home-manager/home.nix
home-manager switch
```

## zsh configs
```
ln zsh/.zshrc ~/.zshrc
```

## vim configs
```
ln vim/.vimrc ~/.vimrc
```

## memo
```
asdf reshim python
```


