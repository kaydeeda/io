# io
# Colors
RESET="\[\e[0m\]"
BOLD="\[\e[1m\]"

# Foreground colors
FG_BLACK="\[\e[30m\]"
FG_RED="\[\e[31m\]"
FG_GREEN="\[\e[32m\]"
FG_YELLOW="\[\e[33m\]"
FG_BLUE="\[\e[34m\]"
FG_MAGENTA="\[\e[35m\]"
FG_CYAN="\[\e[36m\]"
FG_WHITE="\[\e[37m\]"

# Background colors
BG_BLACK="\[\e[40m\]"
BG_RED="\[\e[41m\]"
BG_GREEN="\[\e[42m\]"
BG_YELLOW="\[\e[43m\]"
BG_BLUE="\[\e[44m\]"
BG_MAGENTA="\[\e[45m\]"
BG_CYAN="\[\e[46m\]"
BG_WHITE="\[\e[47m\]"

# Powerline separator glyph
SEPARATOR=$'\uE0B0'  # Try '\u25B6' if this doesn't work in your terminal

# Prompt structure
PS1="${BG_BLUE}${FG_WHITE} \u ${RESET}${BG_CYAN}${FG_BLUE}${SEPARATOR}${BG_CYAN}${FG_WHITE} \w ${RESET}${FG_CYAN}${SEPARATOR} ${RESET}\n\$ "

