# dotfiles_nix

# nix
. "$HOME/.nix-profile/etc/profile.d/hm-session-vars.sh"
. "$HOME/.nix-profile/share/asdf-vm/asdf.sh"
eval "$(direnv hook zsh)"

ln home-manager/home.nix ~/.config/home-manager/home.nix
