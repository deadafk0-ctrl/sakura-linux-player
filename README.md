# sakura-linux-player
A wrapper script to get sakura client running good in linux distributions using wine
## System Prerequisites
because installer is 32 bit app you need to make sure your linux distro has multilib support and wine before running script
### Debian and Ubuntu and Mint and other debian based distros
```bash
sudo dpkg --add-architecture i386
sudo apt update && sudo apt install wine wine32:i386 curl -y
```
### Arch Linux / EndeavourOS / Manjaro

make sure multilib is enabled in /etc/pacman.conf
```bash
sudo pacman -Syu --needed wine curl
```
Fedora / RHEL
```bash
sudo dnf install wine.i686 wine.x86_64 curl -y
```
OpenSUSE 
```bash
sudo zypper install wine curl -y
```
## Installation & usage
once you have your dependencies ready run these commands in terminal to fetch the script and make executable and run the setup:
```bash
curl -L [https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/sakura-linux-player/main/sakura-player](https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/sakura-linux-player/main/sakura-player) -o ~/sakura-player
chmod +x ~/sakura-player
~/sakura-player
```
dont forget to replace YOUR_GITHUB_USERNAME with your actual github username
