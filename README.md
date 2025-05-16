# io
export PS1="\[\e[30;42m\]\u@\h:\w\[\e[0m\]\[\e[97;44m\] \W \[\e[0m\]\ "
# --- COLORS (VIBRANT) ---
RESET="\[\e[0m\]"

# Foreground
FG_BLACK="\[\e[38;5;16m\]"
FG_WHITE="\[\e[38;5;15m\]"

# Backgrounds (Vibrant 256-color)
BG_PURPLE="\[\e[48;5;91m\]"   # Bright magenta
BG_BLUE="\[\e[48;5;33m\]"     # Vivid blue
BG_GREEN="\[\e[48;5;40m\]"    # Bright green
BG_YELLOW="\[\e[48;5;220m\]"  # Vivid yellow
BG_RED="\[\e[48;5;196m\]"     # Bright red
BG_CYAN="\[\e[48;5;51m\]"     # Bright cyan

# Separator
SEPARATOR=$'\uE0B0'  # Nerd Font Powerline glyph

# Prompt structure
PS1=""

# Username segment
PS1+="${BG_PURPLE}${FG_WHITE} \u ${RESET}"
PS1+="${BG_BLUE}${FG_PURPLE}${SEPARATOR}"

# Directory segment
PS1+="${BG_BLUE}${FG_WHITE} \w ${RESET}"
PS1+="${BG_GREEN}${FG_BLUE}${SEPARATOR}"

# Time segment
PS1+="${BG_GREEN}${FG_WHITE} \A ${RESET}"
PS1+="${FG_GREEN}${SEPARATOR} ${RESET}"

# Newline and symbol
PS1+="\n\$ "
