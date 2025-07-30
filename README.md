# Pomo

Pomodoro Timer written in bash.

The script shows a notification when it starts with the time when it will finish, and another one when it finish, and if it's already running you can check until when with the command `pomo`.

![Pomo Start](images/pomo_start.png)

![Pomo Finish](images/pomo_finish.png)

## Requirements

- `at` to schedule commands
    - [at command](https://salsa.debian.org/debian/at)
- `dunst` notifications daemon (you can use any notification daemon)
    - [dunst arch wiki](https://wiki.archlinux.org/title/Dunst)
- `libnotify` library to send notifications (this allows you to use the `notify-send` command)
    - [libnotify arch wiki](https://wiki.archlinux.org/title/Desktop_notifications#Libnotify)

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
# Show the help or other pomodoro sessions running
pomo

# Focus for 60 seconds
pomo 60s

# Focus for 1 hour
pomo 1h
```

To manage the scheduled tasks with `at` use:

```bash
atq # show the jobs scheduled
at -c ID # show the information about a particular job
atrm ID # remove a particular job
```