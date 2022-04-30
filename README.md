# My linux config🍵
These are some useful shell (sh/zh) command aliases which I created for personal use. Anyone can use it. 🐚🔫

Add the below lines to your `~/.bash_aliases` file and `restart` the shell / terminal. ​👨🏻​✈️️​🔁​🏢​

```shell
# Aptitude & System related command aliases.
alias udg="sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade"
alias ud="sudo apt-get update"
alias ug="sudo apt-get upgrade"
alias dg="sudo apt-get dist-upgrade"
alias src="sudo nano /etc/apt/sources.list"
alias gsrc="sudo gedit /etc/apt/sources.list"
alias csrc="sudo cat /etc/apt/sources.list"
alias ver="cat /etc/debian_version"
alias kver="uname -a"
alias cache="sudo apt-get clean"
alias get="sudo apt-get install"
alias yget="sudo apt-get install -y"
alias sget="sudo apt-get install --install-suggests"
alias syget="sudo apt-get install --install-suggests -y"
alias del="sudo apt-get remove"
alias fdel="sudo apt-get remove --purge --autoremove"
alias arem="sudo apt-get autoremove"
alias di="sudo dpkg -i"
alias gi="sudo gdebi"
alias bi="sudo apt-get --fix-broken install"
alias sv="sudo visudo"
alias alt="sudo update-alternatives --config "
alias lssrc="ls /etc/apt/sources.list.d"
alias cdsrc="cd /etc/apt/sources.list.d"
alias lsthm="ls /usr/share/themes/"
alias lsico="ls /usr/share/icons/"
alias cdthm="cd /usr/share/themes/"
alias cdico="cd /usr/share/icons/"
alias grubn="sudo nano /etc/default/grub"
alias grubg="sudo gedit /etc/default/grub"

# Systemctl related command aliases.
alias off="sudo systemctl poweroff"
alias boot="sudo systemctl reboot"
alias sus="sudo systemctl suspend"
alias hib="sudo systemctl hibernate"
alias sstop="sudo systemctl stop"
alias srun="sudo systemctl start"
alias sstat="sudo systemctl status"
alias srest="sudo systemctl restart"
alias son="sudo systemctl enable"
alias soff="sudo systemctl disable"

# Python and pip aliases.
alias python3=python
alias pip3=pip

# Bash related command aliases.
alias brc="sudo nano ~/.bashrc"
alias barc="sudo nano ~/.bash_aliases"
alias carc="cat ~/.bash_aliases"
alias gbrc="sudo gedit ~/.bashrc"
alias gbarc="sudo gedit ~/.bash_aliases"
alias pro="sudo nano ~/.profile"
alias gpro="sudo nano ~/.profile"
# Old limited history size file
# alias past="sudo nano ~/.bash_history"
# alias gpast="gedit ~/.bash_history"
# New unlimited history size file
alias past="sudo nano ~/.bash_eternal_history"
alias gpast="sudo gedit ~/.bash_eternal_history"
alias pd="passwd"
alias spd="sudo passwd"
alias q="exit"

# Miscellaneous & application related command aliases.
alias cls="clear"
alias wi="whereis"
alias wh="which"
alias spm="sudo synaptic"
alias shell="exec $SHELL -l"
alias rem="sudo rm -rf"
alias sun="sudo nano"
alias nvup="curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash"
alias pyeup="cd ~/.pyenv && git pull"
```

# Below are the repositories / mirrors that I use for apt on Debian.

```shell
deb http://deb.debian.org/debian/ bullseye main non-free contrib
deb-src http://deb.debian.org/debian/ bullseye main non-free contrib

# bullseye-updates, to get updates before a point release is made;
# see https://www.debian.org/doc/manuals/debian-reference/ch02.en.html#_updates_and_backports

deb http://security.debian.org/debian-security bullseye-security main contrib non-free
deb-src http://security.debian.org/debian-security bullseye-security main contrib non-free
deb http://ftp.debian.org/debian/ bullseye-backports main contrib non-free
deb-src http://ftp.debian.org/debian/ bullseye-backports main contrib non-free
deb http://deb.debian.org/debian/ bullseye-backports main contrib non-free
deb-src http://deb.debian.org/debian/ bullseye-backports main contrib non-free
deb http://ftp.debian.org/debian/ stretch-backports-sloppy main contrib non-free
deb-src http://ftp.debian.org/debian/ stretch-backports-sloppy main contrib non-free
deb http://deb.debian.org/debian/ bullseye-backports-sloppy main contrib non-free
deb-src http://deb.debian.org/debian/ bullseye-backports-sloppy main contrib non-free
deb http://security.debian.org/ bullseye-security contrib non-free main
deb-src http://security.debian.org/ bullseye-security non-free main contrib
deb http://deb.debian.org/debian/ bullseye-updates contrib non-free main
deb-src http://deb.debian.org/debian/ bullseye-updates non-free main contrib
deb http://deb.debian.org/debian/ bullseye-proposed-updates non-free main contrib
deb-src http://deb.debian.org/debian/ bullseye-proposed-updates non-free main contrib

# The repos below were pickup from debian.pkgs.org when searching for libappindicator1.
deb http://ftp.de.debian.org/debian/ bullseye main contrib non-free
deb-src http://ftp.de.debian.org/debian/ bullseye main contrib non-free
deb http://ftp.de.debian.org/debian/ bullseye-updates main contrib non-free
deb-src http://ftp.de.debian.org/debian/ bullseye-updates main contrib non-free
deb http://ftp.de.debian.org/debian/ bullseye-backports main contrib non-free
deb-src http://ftp.de.debian.org/debian/ bullseye-backports main contrib non-free
deb http://ftp.de.debian.org/debian/ bullseye-proposed-updates main contrib non-free
deb-src http://ftp.de.debian.org/debian/ bullseye-proposed-updates main contrib non-free
deb http://ftp.de.debian.org/debian/ bullseye-backports-sloppy main contrib non-free
deb-src http://ftp.de.debian.org/debian/ bullseye-backports-sloppy main contrib non-free

# Ubuntu based dependencies required for debian.
# Always disable the below four repositories when
# updating system for the first time after every fresh install.
# And later re-enable it and do a ud and udg or just udg if you'd like to.
# deb http://archive.ubuntu.com/ubuntu focal main multiverse restricted universe
# deb-src http://archive.ubuntu.com/ubuntu focal main multiverse restricted universe
# deb http://archive.ubuntu.com/ubuntu focal-backports main multiverse restricted universe
# deb-src http://archive.ubuntu.com/ubuntu focal-backports main multiverse restricted universe

# Ubuntu - US (342 Gbps)
# deb http://mirror.enzu.com/ubuntu/ focal main multiverse restricted universe
# deb-src http://mirror.enzu.com/ubuntu/ focal main multiverse restricted universe
# deb http://mirror.enzu.com/ubuntu/ focal-backports main multiverse restricted universe
# deb-src http://mirror.enzu.com/ubuntu/ focal-backports main multiverse restricted universe
# deb http://mirror.genesisadaptive.com/ubuntu/ focal main multiverse restricted universe
# deb-src http://mirror.genesisadaptive.com/ubuntu/ focal main multiverse restricted universe
# deb http://mirror.genesisadaptive.com/ubuntu/ focal-backports main multiverse restricted universe
# deb-src http://mirror.genesisadaptive.com/ubuntu/ focal-backports main multiverse restricted universe
# deb http://mirror.math.princeton.edu/pub/ubuntu/ focal main multiverse restricted universe
# deb-src http://mirror.math.princeton.edu/pub/ubuntu/ focal main multiverse restricted universe
# deb http://mirror.math.princeton.edu/pub/ubuntu/ focal-backports main multiverse restricted universe
# deb-src http://mirror.math.princeton.edu/pub/ubuntu/ focal-backports main multiverse restricted universe
# deb http://mirror.pit.teraswitch.com/ubuntu/ focal main multiverse restricted universe
# deb-src http://mirror.pit.teraswitch.com/ubuntu/ focal main multiverse restricted universe
# deb http://mirror.pit.teraswitch.com/ubuntu/ focal-backports main multiverse restricted universe
# deb-src http://mirror.pit.teraswitch.com/ubuntu/ focal-backports main multiverse restricted universe

# Ubuntu - UK - 73 Gbps
# deb http://mirror.cov.ukservers.com/ubuntu/ focal main multiverse restricted universe
# deb-src http://mirror.cov.ukservers.com/ubuntu/ focal main multiverse restricted universe
# deb http://mirror.cov.ukservers.com/ubuntu/ focal-backports main multiverse restricted universe
# deb-src http://mirror.cov.ukservers.com/ubuntu/ focal-backports main multiverse restricted universe

# Debian - sid, testing
# deb http://deb.debian.org/debian/ sid main contrib non-free
# deb http://deb.debian.org/debian/ testing main contrib non-free
# deb http://deb.debian.org/debian/ testing-updates main contrib non-free
# deb http://deb.debian.org/debian-security testing-security main

# Custom-server mirrors apart from the main-server ones, considered above.
# World-wide countries mirrors
# Enable when needed.

# Australia 
# deb http://debian.mirror.serversaustralia.com.au/debian/ bullseye main non-free contrib
# deb http://debian.mirror.serversaustralia.com.au/debian/ bullseye-updates main non-free contrib
# deb http://debian.mirror.serversaustralia.com.au/debian/ bullseye-proposed-updates main non-free contrib
# deb http://debian.mirror.serversaustralia.com.au/debian/ bullseye-backports main non-free contrib
# deb http://debian.mirror.serversaustralia.com.au/debian/ bullseye-backports-sloppy main non-free contrib

# Austria
# deb http://ftp.at.debian.org/debian/ bullseye main non-free contrib
# deb http://ftp.at.debian.org/debian/ bullseye-updates main non-free contrib
# deb http://ftp.at.debian.org/debian/ bullseye-proposed-updates main non-free contrib
# deb http://ftp.at.debian.org/debian/ bullseye-backports main non-free contrib
# deb http://ftp.at.debian.org/debian/ bullseye-backports-sloppy main non-free contrib

# New Zealand
# deb http://mirror.fsmg.org.nz/debian/ bullseye main non-free contrib
# deb http://mirror.fsmg.org.nz/debian/ bullseye-updates main non-free contrib
# deb http://mirror.fsmg.org.nz/debian/ bullseye-proposed-updates main non-free contrib
# deb http://mirror.fsmg.org.nz/debian/ bullseye-backports main non-free contrib
# deb http://mirror.fsmg.org.nz/debian/ bullseye-backports-sloppy main non-free contrib

# China
# deb https://mirrors.ustc.edu.cn/debian/ bullseye main non-free contrib
# deb https://mirrors.ustc.edu.cn/debian/ bullseye-updates main non-free contrib
# deb https://mirrors.ustc.edu.cn/debian/ bullseye-proposed-updates main non-free contrib
# deb https://mirrors.ustc.edu.cn/debian/ bullseye-backports main non-free contrib
# deb https://mirrors.ustc.edu.cn/debian/ bullseye-backports-sloppy main non-free contrib

# CZech Republic
# deb http://ftp.cz.debian.org/debian/ bullseye main non-free contrib
# deb http://ftp.cz.debian.org/debian/ bullseye-updates main non-free contrib
# deb http://ftp.cz.debian.org/debian/ bullseye-proposed-updates main non-free contrib
# deb http://ftp.cz.debian.org/debian/ bullseye-backports main non-free contrib
# deb http://ftp.cz.debian.org/debian/ bullseye-backports-sloppy main non-free contrib

# Germany
# deb http://ftp.uni-stuttgart.de/debian/ bullseye main non-free contrib
# deb http://ftp.uni-stuttgart.de/debian/ bullseye-updates main non-free contrib
# deb http://ftp.uni-stuttgart.de/debian/ bullseye-proposed-updates main non-free contrib
# deb http://ftp.uni-stuttgart.de/debian/ bullseye-backports main non-free contrib
# deb http://ftp.uni-stuttgart.de/debian/ bullseye-backports-sloppy main non-free contrib

# Russia
# deb http://mirror.docker.ru/debian/ bullseye main non-free contrib
# deb http://mirror.docker.ru/debian/ bullseye-updates main non-free contrib
# deb http://mirror.docker.ru/debian/ bullseye-proposed-updates main non-free contrib
# deb http://mirror.docker.ru/debian/ bullseye-backports main non-free contrib
# deb http://mirror.docker.ru/debian/ bullseye-backports-sloppy main non-free contrib

# Ukraine
# deb http://debian.netforce.hosting/debian/ bullseye main non-free contrib
# deb http://debian.netforce.hosting/debian/ bullseye-updates main non-free contrib
# deb http://debian.netforce.hosting/debian/ bullseye-proposed-updates main non-free contrib
# deb http://debian.netforce.hosting/debian/ bullseye-backports main non-free contrib
# deb http://debian.netforce.hosting/debian/ bullseye-backports-sloppy main non-free contrib

# United Kingdom
# deb http://mirror.ox.ac.uk/debian/ bullseye main non-free contrib
# deb http://mirror.ox.ac.uk/debian/ bullseye-updates main non-free contrib
# deb http://mirror.ox.ac.uk/debian/ bullseye-proposed-updates main non-free contrib
# deb http://mirror.ox.ac.uk/debian/ bullseye-backports main non-free contrib
# deb http://mirror.ox.ac.uk/debian/ bullseye-backports-sloppy main non-free contrib

# United states
# deb http://mirror.siena.edu/debian/ bullseye main non-free contrib
# deb http://mirror.siena.edu/debian/ bullseye-updates main non-free contrib
# deb http://mirror.siena.edu/debian/ bullseye-proposed-updates main non-free contrib
# deb http://mirror.siena.edu/debian/ bullseye-backports main non-free contrib
# deb http://mirror.siena.edu/debian/ bullseye-backports-sloppy main non-free contrib

# Microsoft Debian repositories
deb https://packages.microsoft.com/debian/11/prod bullseye main
deb https://packages.microsoft.com/debian/11/prod insiders-slow main
deb https://packages.microsoft.com/debian/11/prod nightly main
```

✨

Cheers ! 🥂
