# Arch Configuration for dmenu, dwm, and st

This repository contains my personal configuration files for dmenu, dwm, and st on Arch Linux. These configurations have been tailored to my specific needs and preferences, and they may serve as a useful starting point for others looking to customize their Arch setup.

## Features

- Custom keybindings for efficient workflow
- Optimized color schemes for better readability
- Additional patches for extended functionality

## Prerequisites

Before you can use these configurations, ensure that you have the following installed on your Arch Linux system:

- `base-devel` package group
- `git`
- `xorg-server`
- `xorg-xinit`

## Installation

1. Clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/arch-config.git
```

2. Change to the cloned directory:

```bash
cd arch-config
```
3. Compile and install each application:
### dmenu
```bash
cd dmenu
sudo make clean install
```
### dmw
```bash
cd ../dwm
sudo make clean install
```
### st
```bash
cd ../st
sudo make clean install
```

4. Create or update your .xinitrc file in your home directory to start dwm on login:
 ```bash
echo "exec dwm" > ~/.xinitrc
```
5. Restart your X session or reboot your system to apply the changes.

## Customization
Feel free to explore the configuration files and make changes to suit your needs. Each application's directory contains a config.h file where you can modify settings, keybindings, and more.
If you make any changes, be sure to recompile and reinstall the affected application(s) using the sudo make clean install command.
## Acknowledgments
- The suckless community for creating and maintaining dmenu, dwm, and st
- Various patch authors for their contributions to extending the functionality of these applications
