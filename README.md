# Bash-aliases 🍵
These are some useful shell (sh/zh) command aliases which, I suppose will be help to y'all as well. 🐚🔫

Add the below lines to your `~/.bash_aliases` file and `restart` the shell / terminal. ​👨🏻​✈️️​🔁​🏢​

```shell
# Aptitude & System related command aliases.
alias udg="sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade"
alias ud="sudo apt-get update"
alias ug="sudo apt-get upgrade"
alias dg="sudo apt-get dist-upgrade"
alias src="sudo nano /etc/apt/sources.list"
alias gsrc="sudo gedit /etc/apt/sources.list"
alias ver="cat /etc/debian_version"
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
alias gbrc="sudo gedit ~/.bashrc"
alias gbarc="sudo gedit ~/.bash_aliases"
alias pro="sudo nano ~/.profile"
alias gpro="sudo nano ~/.profile"
alias past="sudo nano ~/.bash_history"
alias gpast="gedit ~/.bash_history"
alias pd="passwd"
alias spd="sudo passwd"
alias q="exit"

# Miscellaneous & application related command aliases.
alias cs="clear"
alias wi="whereis"
alias wh="which"
alias spm="sudo synaptic"
alias shell="exec $SHELL -l"
alias rem="sudo rm -rf"
alias sun="sudo nano"
alias calup="sudo -v && wget -nv -O- https://download.calibre-ebook.com/linux-installer.sh | sudo sh /dev/stdin"
alias jopup="wget -O - https://raw.githubusercontent.com/laurent22/joplin/dev/Joplin_install_and_update.sh | bash"
alias nvup="curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash"
```

Will keep adding if I pertain to create more of such.✨

Cheers ! 🥂
