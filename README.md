# ThinkPad Theme for GRUBv2

## Set up

1. Make themes folder in /boot/grub/
```
sudo mkdir /boot/grub/themes
```
2. Download or clone the code.
```
git clone https://github.com/duncanldaho/GRUB-ThinkPad && cd GRUB-ThinkPad
```
2. From inside of the project directory, copy the theme to grub.
```
sudo cp -r ThinkPad /boot/grub/themes/
```
## Activating Themes

1. After set up, use your preferred editor to update the GRUB config file.
```
vim /etc/default/grub
OR
nano /etc/default/grub
```
2. Update the following lines, replace [RESOLUTION] with your screen size
   (1920x1080 or 1680x1050).
```
GRUB_THEME=/boot/grub/themes/ThinkPad/theme.txt
GRUB_GFXMODE=[RESOLUTION]
```
