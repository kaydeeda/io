# io
export PS1="\[\e[30;42m\]\u@\h:\w\[\e[0m\]\[\e[97;44m\] \W \[\e[0m\]\ "
# --- RESET ---
RESET="\[\e[0m\]"

# --- Colors (Foreground) ---
FG_WHITE="\[\e[38;5;15m\]"
FG_BLACK="\[\e[38;5;16m\]"
FG_BLUE="\[\e[38;5;33m\]"
FG_PURPLE="\[\e[38;5;91m\]"
FG_GREEN="\[\e[38;5;40m\]"

# --- Colors (Backgrounds) ---
BG_PURPLE="\[\e[48;5;91m\]"
BG_BLUE="\[\e[48;5;33m\]"
BG_GREEN="\[\e[48;5;40m\]"

# --- Separator Glyph (Nerd Font Powerline) ---
SEPARATOR=$'\uE0B0'

# --- Prompt Construction ---
PS1=""

# 1. Username segment
PS1+="${BG_PURPLE}${FG_WHITE} \u "  # username block
PS1+="${FG_PURPLE}${BG_BLUE}${SEPARATOR}"  # separator pointing to next block

# 2. Directory segment
PS1+="${BG_BLUE}${FG_WHITE} \w "  # current working directory
PS1+="${FG_BLUE}${BG_GREEN}${SEPARATOR}"  # separator pointing to next block

# 3. Time segment
PS1+="${BG_GREEN}${FG_WHITE} \A "  # current time (HH:MM)
PS1+="${RESET}${FG_GREEN}${SEPARATOR}"  # final separator pointing to RESET

# Newline and prompt symbol
PS1+="\n\$ "
