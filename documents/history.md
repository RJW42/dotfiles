pacman -S 1password firefox neovim base-devel lua man-db man-pages discord unzip

## Man
# https://unix.stackexchange.com/questions/663575/how-can-i-make-sure-that-man-has-pages-installed
mandb

## Yay
# https://linuxiac.com/how-to-install-aur-packages-in-arch-linux/

## Nord VPN
# https://wiki.archlinux.org/title/NordVPN
groupadd -r nordvpn
usermod -aG nordvpm $USER
yay nordvpn-gui

## NeoVim
git clone --depth 1 https://github.com/wbthomason/packer.nvim ~/.local/share/nvim/site/pack/packer/start/packer.nvim
nvim +PackerSync

## Audio 
sudo pacman -S pipewire-pulse pipewire-audio pipewire-alsa wireplumber pipewire-jack pavucontrol
sudo yay coppwr 

# https://www.siberoloji.com/how-to-configure-pipewire-for-audio-on-arch-linux/
# Non Sudo
systemctl --user enable --now pipewire pipewire-pulse wireplumber


## Hyperland
sudo pacman -S hyprlock
yay -S hyprpaper
yay -Ss waybar
yay -S waybar

## Projects 
rustup default stable

mkdir -p documents/projects downloads pictures/required

git clone git@github.com:RJW42/tts.git $HOME/documents/projects/tts
git clone git@github.com:RJW42/brick.git $HOME/documents/projects/brick

## Steam
https://wiki.archlinux.org/title/Steam
