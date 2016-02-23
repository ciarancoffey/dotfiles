# dotfiles
Just personal dotfiles


    PS1=\[\033[35m\]\t\[\033[m\]-\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[36m\]$(__git_ps1 " (%s)")\[\033[33;1m\]$\[\033[m\]
    
Results in:

    09:31:13-ccoffey@ciaranc:~/aws-logging-infrastructure/cloudformation (master)$

Purple time, white dash, blue username, white @, green hostname:, yellow path, space, blue git branch if exists, yellow $, space.
Possibly a bit long. Requires /usr/share/git/completion/git-prompt.sh to be sourced.
