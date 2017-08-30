apt-get install xsel xclip screen

add to .bashrc - 

export VISUAL=vim
export EDITOR="$VISUAL"

export TERM="xterm-256color"

if command -v tmux>/dev/null; then
          [[ ! $TERM =~ screen ]] && [ -z $TMUX ] && exec tmux
fi
