# sakura-linux-player

sakura.mba for working in wine in your Linux. Sakura Linux Launcher is the first automated, multi-architecture Wine wrapperscript with download, build and run functionalities for the Sakura client on various architectures and Linux distributions.

System requirements

The Sakura client installer is an 32-bit Windows application that is designed to be a 32-bit Windows application that temporarily runs on your Linux system. Your Linux operating system therefore needs support for a 32-bit architecture (multilib) with the required installations of both Wine and Curl. Please refer below to how you can set it up for your specific distro before you run the script!

Debian / Ubuntu / Linux Mint / Pop! _OS

Bash

sudo dpkg --add-architecture i386

sudo apt update

sudo apt install wine wine32:i386 curl -y

Arch Linux / EndeavourOS / Manjaro

Bash

Enable the [multilib] repository in your /etc/pacman.conf first.
Sudo pacman -Syu --needed wine curl

Fedora / Red Hat Enterprise Linux (RHEL)

Bash

sudo dnf install wine.i686 wine.x86_64 curl -y

OpenSUSE (Tumbleweed / Leap)

Bash

sudo zypper install wine curl -y

Installation and setup

Once all prerequisites for your system have been satisfied, you can download and install Sakura. Simply run the following two commands:

Bash

curl -L https://raw.githubusercontent.com/YOURGITHUBUSERNAME/sakura-linux-player/main/sakura-player -o ~/sakura-player

chmod +x ~/sakura-player

~/sakura-player

Before you continue reading on and install it…

Do not forget to replace ‘YOURGITHUBUSERNAME‘ in the installation snippet above! It’s currently pointing to your default GitHub username which will result in an error if you haven’t created the repo yet in which this project will live, or if it’s not named exactly this. This line of code should fetch your actual GitHub profile name from GitHub so we can pull the files down successfully when you eventually update this repo to its “full public version”.
