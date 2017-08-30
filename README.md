apt-get install xsel xclip screen

install fpp https://github.com/facebook/PathPicker/releases/tag/0.7.2

add to .bashrc - 

export VISUAL=vim
export EDITOR="$VISUAL"

export TERM="xterm-256color"

if command -v tmux>/dev/null; then
          [[ ! $TERM =~ screen ]] && [ -z $TMUX ] && exec tmux
fi
