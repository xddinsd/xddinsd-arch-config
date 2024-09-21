# xddinsd-arch-config
My command set to configure arch from scratch

### First of all, install arch
* f2fs for SSD
* pipewire
* networkmanager
* multilib

### Install ML4W config:
```bash
nmcli d wifi connect <wifi_name> password <password>

sudo pacman -Syu
# Install yay
sudo pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si
# config:
yay -S ml4w-hyprland
ml4w-hyprland-setup
```

### Add other packages:
```
# apps
yay -S code qsynth telegram-desktop
flatpak install steam vesktop zoom
# utils
yay -S game-devices-udev
# code
yay -S python-pip 
