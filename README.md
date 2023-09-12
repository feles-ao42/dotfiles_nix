# Nix version dotfiles

## nix
https://nixos.org/download#nix-install-macos

```
sh <(curl -L https://nixos.org/nix/install)
```
## shell's

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
. "$HOME/.nix-profile/etc/profile.d/hm-session-vars.sh"
. "$HOME/.nix-profile/share/asdf-vm/asdf.sh"
eval "$(direnv hook zsh)"
```

```
rm ~/.config/home-manager/home.nix
ln home-manager/home.nix ~/.config/home-manager/home.nix
home-manager switch
```

## memo
```
asdf reshim python
```


