# io
export PS1="\[\e[30;42m\]\u@\h:\w\[\e[0m\]\[\e[97;44m\] \W \[\e[0m\]\ "


# Reset
RESET="\[\e[0m\]"

# Foregrounds
FG_WHITE="\[\e[38;5;15m\]"

# Backgrounds (vibrant)
BG_PURPLE="\[\e[48;5;91m\]"   # Segment 1
BG_BLUE="\[\e[48;5;33m\]"     # Segment 2
BG_GREEN="\[\e[48;5;40m\]"    # Segment 3
BG_GRAY="\[\e[48;5;236m\]"    # Final segment (or trailing)

# Separator
SEPARATOR=$'\uE0B0'  # Nerd Font triangle

# Build Prompt
PS1=""

# Segment: Username
PS1+="${BG_PURPLE}${FG_WHITE} \u "
PS1+="${FG_PURPLE}${BG_BLUE}${SEPARATOR}"

# Segment: Directory
PS1+="${BG_BLUE}${FG_WHITE} \w "
PS1+="${FG_BLUE}${BG_GREEN}${SEPARATOR}"

# Segment: Time
PS1+="${BG_GREEN}${FG_WHITE} \A "
PS1+="${FG_GREEN}${BG_GRAY}${SEPARATOR}"

# Segment: trailing filler (gray block)
PS1+="${BG_GRAY} ${RESET}"

# Newline and prompt symbol
PS1+="\n\$ "
