# Pomo

Pomodoro Timer written in bash.

## Requirements

- `at` to schedule commands
    - [at command](https://salsa.debian.org/debian/at)
- `dunst` to send notifications
    - [dunst arch wiki](https://wiki.archlinux.org/title/Dunst)

**Note**: The script make use of `notify-send` so be sure to have it on your system.

## Installation

You can clone the whole repository.

```bash
# Clone the repo
git clone https://github.com/bash-bunny/pomo_timer.git
# Move it the script to your PATH
mv pomo ~/.local/bin
# Give it permissions
chmod u+x ~/.local/bin/pomo
```

Or you can just download the bash script.

```bash
# Download the script
curl -sSLOfk https://raw.githubusercontent.com/bash-bunny/pomo_timer/refs/heads/main/pomo
# Move it to your PATH
mv pomo ~/.local/bin
# Give it permissions
chmod u+x pomo
```

## Usage

```bash
# Show the help
pomo

# Focus for 60 seconds
pomo 60s

# Focus for 1 hour
pomo 1h
```