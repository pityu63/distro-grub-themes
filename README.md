# Distro Grub Themes
[![name](https://img.shields.io/github/license/AdisonCavani/distro-grub-themes)](https://github.com/AdisonCavani/distro-grub-themes/blob/master/LICENSE) [![name](https://img.shields.io/badge/Donate-PayPal-blue)](https://www.paypal.com/donate/?hosted_button_id=TKVET8LGHH5SG)

A pack of GRUB2 themes for different Linux distribution.<br>
It aims to replace default Grub look, with nice and colorful theme.

## Supported distributions
- Arch Linux
- Debian
- ElementaryOS
- Fedora
- Linux Mint
- Manjaro
- openSUSE
- Pop! OS
- Solus
- Ubuntu
- Ventoy

## Preview theme

<p float="left">
<img src="https://raw.githubusercontent.com/AdisonCavani/grub-theme/master/preview/Arch%20Linux.png" width="49%"/>
<img src="https://raw.githubusercontent.com/AdisonCavani/grub-theme/master/preview/Debian.png" width="49%"/>
</p>
<p float="left">
<img src="https://raw.githubusercontent.com/AdisonCavani/grub-theme/master/preview/ElementaryOS.png" width="49%"/>
<img src="https://raw.githubusercontent.com/AdisonCavani/grub-theme/master/preview/Fedora.png" width="49%"/>
</p>
<p float="left">
<img src="https://raw.githubusercontent.com/AdisonCavani/os-grub-themes/master/preview/Linux%20Mint.png" width="49%"/>
<img src="https://raw.githubusercontent.com/AdisonCavani/os-grub-themes/master/preview/Manjaro.png" width="49%"/>
</p>
<p float="left">
<img src="https://raw.githubusercontent.com/AdisonCavani/os-grub-themes/master/preview/openSUSE.png" width="49%"/>
<img src="https://raw.githubusercontent.com/AdisonCavani/os-grub-themes/master/preview/popOS.png" width="49%"/>
</p>
<p float="left">
<img src="https://raw.githubusercontent.com/AdisonCavani/os-grub-themes/master/preview/Solus.png" width="49%"/>
<img src="https://raw.githubusercontent.com/AdisonCavani/os-grub-themes/master/preview/Ubuntu.png" width="49%"/>
</p>

## Installation via Grub Customizer

In order to clone repository from Github you have to install `git` package <br>
Alternatively you can download zip package - **Code -> Download ZIP**

#### Clone the repository
You can clone repository or go to [release page](https://github.com/AdisonCavani/distro-grub-themes/releases) and download a single theme
```
git clone https://github.com/AdisonCavani/distro-grub-themes.git
```

### Install Grub Customizer

Apt
```
sudo add-apt-repository ppa:danielrichter2007/grub-customizer
sudo apt-get update
sudo apt-get install grub-customizer
```
Pacman
```
sudo pacman -S grub-customizer
```

Dnf
```
sudo dnf install grub-customizer
```

Eopkg
```
sudo eopkg install grub-customizer
```
### Install pre-made theme with Grub Customizer

- Open Grub Customizer
- Go to **Appearance settings** tab
- Select *Custom resolution* and type in your resolution. E.g: 1920x1080
- Press *Add theme* button, go to your directory, where you have cloned repository. In my case `/home/adison/distro-grub-theme`
- Select your theme located in `/themes` directory
- Save changes

### Install custom-made theme with Grub Customizer

- Edit your theme located in `/customize` folder
- With your file manager, inside edited theme directory, select all files and **create archive** with .tar or .tar.xz extension
- Open Grub Customizer
- Go to **Appearance settings** tab
- Select *Custom resolution* and type in your resolution. E.g: 1920x1080
- Press *Add theme* button, go to your directory, where you have cloned repository. In my case `/home/adison/distro-grub-theme`
- Change view settings from *Archive files* to **All files**
- Select your archive
- Save changes


## Manual Installation

In order to clone repository from Github you have to install `git` package <br>
Alternatively you can download zip package - **Code -> Download ZIP**

#### Clone the repository
You can clone repository or go to [release page](https://github.com/AdisonCavani/distro-grub-themes/releases) and download a single theme
```
git clone https://github.com/AdisonCavani/distro-grub-themes.git
```

#### Create themes directory
```
sudo mkdir /boot/grub/themes
```

#### Edit or use pre-made theme
```
cd distro-grub-themes/customize
```

#### Copy theme
Theme must be unpacked (in folder)
```
sudo cp -r Ubuntu/ /boot/grub/themes
```

#### Edit Grub config
You can use your favourite text editor
```
sudo nano /etc/default/grub
```
Uncomment this line and set your resolution:
```
GRUB_GFXMODE=1920x1080
```

At the end of file add theme path:
```
GRUB_THEME="/boot/grub/themes/Ubuntu/theme.txt"
```
Replace "Ubuntu" with selected theme<br>
Ctrl+O to save, Ctrl+X to exit

## To-do list
Feature | Status
------------ | -------------
4K & 2K displays support | In dev
Ultrawide display support | In future dev
Gentoo theme | In dev
KDE Neon theme | In dev
Slackware theme | In dev
