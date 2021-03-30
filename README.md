# Linux Terminal

Short manual to setup a nice and usefull linux terminal. This was tested on Ubuntu 18.04 and 20.04.

## Install vim and terminator

`sudo apt-get -y install vim terminator`

## Customize terminator

To customize terminator, open the app and right click on it.

Disable "Windows borders"

![Terminator 1](https://github.com/juanccq/linux-terminal/blob/main/images/selection_001.png?raw=true)

Disable "Show titlebar" and change the default font to "Ubuntu Mono Regular 11"

![Terminator 2](https://github.com/juanccq/linux-terminal/blob/main/images/selection_002.png?raw=true)

Change the window transparency

![Terminator 3](https://github.com/juanccq/linux-terminal/blob/main/images/selection_003.png?raw=true)

## Install the required libraries for Zsh

`sudo apt install -y curl wget git`

## Install Zsh

`sudo apt install -y zsh`

## Install oh-my-zsh

`sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Install plugins for oh-my-zsh

`git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions`

`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting`

## Edit the zshrc file

`vim .zshrc`

### Change the theme to Agnoster

`ZSH_THEME="agnoster"`

### Enable plugins for the terminal

`plugins=(git git-extras docker zsh-autosuggestions zsh-syntax-highlighting)`

### Edit the theme to add a time mark in the prompt

`vim .oh-my-zsh/themes/agnoster.zsh-theme`

Add this line at the end of the file

`RPROMPT="[%D{%y/%m/%f}|%@]"`

## Useful links

Terminator shortcuts [https://cheatography.com/elpedro/cheat-sheets/terminator/](https://cheatography.com/elpedro/cheat-sheets/terminator/)

Git plugins shortcuts [https://dev.to/giulia_chiola/oh-my-zsh-cheatsheet-3all](https://dev.to/giulia_chiola/oh-my-zsh-cheatsheet-3all)
