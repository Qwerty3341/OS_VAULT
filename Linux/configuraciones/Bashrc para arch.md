#PS1='[\u@\h \W]\$ '
PS1='[\[\e[32m\]\u@\h\[\e[0m\] \[\e[34m\]\W\[\e[0m\]]\[\e[33m\]\$\[\e[0m\] '

# =======
# Configs
# =======

export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init - bash)"

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion


export EDITOR=vim

alias ll='ls -la'
alias open=xdg-open
alias arch='uname -m'
