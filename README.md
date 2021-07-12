# Reimagined-sniffle 🍵
These are some useful shell (sh/zh) command aliases that I created which, I suppose will be help to y'all as well. 🐚🔫

Add the below lines to your `~/.bashrc` file and `restart` the shell / terminal. ​👨🏻​✈️️​🔁​🏢​

```shell
# Aptitude & System related command aliases.
alias udg="sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade"
alias ud="sudo apt-get update"
alias ug="sudo apt-get upgrade"
alias dg="sudo apt-get dist-upgrade"
alias src="sudo nano /etc/apt/sources.list"
alias ver="cat /etc/debian_version"
alias cache="sudo apt-get clean"
alias get="sudo apt install"
alias del="sudo apt-get remove"
alias fdel="sudo apt-get remove --purge --autoremove"
alias di="sudo dpkg -i"
alias sv="sudo visudo"
alias alt="sudo update-alternatives --config "

# Systemctl related command aliases.
alias off="sudo systemctl poweroff"
alias boot="sudo systemctl reboot"
alias sus="sudo systemctl suspend"
alias hib="sudo systemctl hibernate"
alias servstop="sudo systemctl stop"
alias servrun="sudo systemctl start"
alias servstat="sudo systemctl status"
alias servrest="sudo systemctl restart"
alias servon="sudo systemctl enable"
alias servoff="sudo systemctl disable"
alias aptconf="sudo nano /etc/apt/sources.list"

# Python and pip aliases by prithvi.
alias python3=python
alias pip3=pip

# Bash related command aliases.
alias brc="sudo nano ~/.bashrc"
alias gbrc="sudo gedit ~/.bashrc"
alias form="sudo nano ~/.profile"
alias past="sudo nano ~/.bash_history"

# Miscellaneous & application related command aliases.
alias cls="clear"
alias ex="exit"
alias wi="whereis"
alias wh="which"
alias spm="sudo synaptic"
alias shell="exec $SHELL"
alias code="code-insiders"
alias rem="sudo rm -rf"
alias sun="sudo nano"
```

Will keep adding if I pertain to create more of such.✨

Cheers ! 🥂
