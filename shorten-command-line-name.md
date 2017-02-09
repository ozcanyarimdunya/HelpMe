## Ubuntu .bashrc settings to shorten command line name


### This is for root:
    PS1='${debian_chroot:+($debian_chroot)}\[\e[36m\](\[\e[31m\]root\[\e[36m\])\[\e[94m\]~\[\e[01;32m\]$\[\e[00m\] '

-----

### This is for user:
    PS1='${debian_chroot:+($debian_chroot)}\[\033[01;34m\]~\[\033[01;32m\]$\[\033[00m\] '
