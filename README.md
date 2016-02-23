# dotfiles
Just personal dotfiles, this repo mainly serves as a backup for me.

####PS1

I've had this PS1 for awhile and tweaked it where I almost like it

    PS1=\[\033[35m\]\t\[\033[m\]-\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[36m\]$(__git_ps1 " (%s)")\[\033[33;1m\]$\[\033[m\]
    
Results in:

![alt text](https://ccoffey.ie/Images/PS1.jpg "PS1 example")

    09:45:56-ccoffey@ciaranc:~/logging-hub (release)$

Purple time, white dash, blue username, white @, green hostname:, yellow path, space, blue git branch if exists, yellow $, space.
Possibly a bit long. Requires /usr/share/git/completion/git-prompt.sh to be sourced.


####Aliases

Some sane settings for rdesktop, based on my monitor size in work and with copy & paste

    alias rd='rdesktop -g 1000x850  -r clipboard:CLIPBOARD'
    
The cisco gear I currenly interact with (read: old stuff) does not work by default with current openssh client, The diffie-hellman sha1 key exchange needs to specified

    alias cisco-ssh='ssh -oKexAlgorithms=+diffie-hellman-group1-sha1'
    
    


