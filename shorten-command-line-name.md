## Ubuntu .bashrc settings to shorten command line name


### This is for root:
    PS1='${debian_chroot:+($debian_chroot)}\[\e[36m\](\[\e[31m\]root\[\e[36m\])\[\e[94m\]~\[\e[01;32m\]$\[\e[00m\] '
or
    
    ###################################################
      #						#
      #	  CUSTOM COLOR BY @OZCANYARIMDUNYA	#
      #						#
    ###################################################

    COLOR_BLACK=$(tput setaf 0)
    COLOR_RED=$(tput setaf 1)
    COLOR_GREEN=$(tput setaf 2)
    COLOR_YELLOW=$(tput setaf 3)
    COLOR_BLUE=$(tput setaf 4)
    COLOR_MAGENTA=$(tput setaf 5)
    COLOR_CYAN=$(tput setaf 6)
    COLOR_WHITE=$(tput setaf 7)
    COLOR_RESET=$(tput sgr0)

    if [ "$color_prompt" = yes ]; then
        PS1='\n${debian_chroot:+($debian_chroot)}$COLOR_BLUE•$COLOR_RED•$COLOR_GREEN•$COLOR_RESET '
    else
        PS1='\n${debian_chroot:+($debian_chroot)}$COLOR_BLUE•$COLOR_RED•$COLOR_GREEN•$COLOR_RESET '
    fi

-----

### This is for user:
    PS1='${debian_chroot:+($debian_chroot)}\[\033[01;34m\]~\[\033[01;32m\]$\[\033[00m\] '
or
    
    ###################################################
      #						#
      #	  CUSTOM COLOR BY @OZCANYARIMDUNYA	#
      #						#
    ###################################################

    COLOR_BLACK=$(tput setaf 0)
    COLOR_RED=$(tput setaf 1)
    COLOR_GREEN=$(tput setaf 2)
    COLOR_YELLOW=$(tput setaf 3)
    COLOR_BLUE=$(tput setaf 4)
    COLOR_MAGENTA=$(tput setaf 5)
    COLOR_CYAN=$(tput setaf 6)
    COLOR_WHITE=$(tput setaf 7)
    COLOR_RESET=$(tput sgr0)

    if [ "$color_prompt" = yes ]; then
        PS1='\n${debian_chroot:+($debian_chroot)}$COLOR_BLUE•$COLOR_RED•$COLOR_YELLOW•$COLOR_RESET '
    else
        PS1='\n${debian_chroot:+($debian_chroot)}$COLOR_BLUE•$COLOR_RED•$COLOR_YELLOW•$COLOR_RESET '
    fi
