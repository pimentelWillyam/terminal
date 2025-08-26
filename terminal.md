# 🎨 Prompt personalizado estilo Dracula
export PS1="\[\e[0;35m\]\u@\h:\[\e[0;36m\]\w\[\e[0;32m\] \$ \[\e[0m\]"

# 🎯 Banner Dracula + Neofetch

if command -v neofetch > /dev/null; then
  neofetch | lolcat
fi
if command -v figlet > /dev/null && command -v lolcat > /dev/null; then
  figlet -d ~/.figlet -f ansi_shadow "Willyam" | lolcat
fi


# 🔧 Aliases
alias ll='ls -la --color=auto'
alias gs='git status'
alias cls='clear'
alias ..='cd ..'

#SDKMAN
export SDKMAN_DIR="$HOME/.sdkman"
[[ -s "$HOME/.sdkman/bin/sdkman-init.sh" ]] && source "$HOME/.sdkman/bin/sdkman-init.sh"