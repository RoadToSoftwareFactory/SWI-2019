parse_git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
# git branch 2>/dev/null | /usr/bin/grep '^*' | colrm 1 2)"
}

PS1_date="\[\033[38;5;237m\]\d\[$(tput sgr0)\]\[\033[38;5;15m\]"
PS1_time="\[$(tput sgr0)\]\[\033[38;5;236m\]\t\[$(tput sgr0)\]\[\033[38;5;15m\]"
PS1_wdir="\[$(tput sgr0)\]\[\033[38;5;24m\]\W"
PS1_gitbranch="\e[38;5;204m\]\$(parse_git_branch)"
PS1_gt="\[$(tput bold)\]\[$(tput sgr0)\]\[\e[38;5;214m\]>"
PS1_other="\[$(tput sgr0)\]\[$(tput sgr0)\]\[\e[38;5;15m\]"

export PS1="${PS1_date} ${PS1_time} ${PS1_wdir}${PS1_gitbranch}${PS1_gt}${PS1_other} \[$(tput sgr0)\]"

