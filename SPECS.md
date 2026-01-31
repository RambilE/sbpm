# This file describes specifications for packages for sbpm
This is reflected in the github.com/rambile/sbpm-test

# rampkg
rampkg is a bash script that specifies dependencies to install and where to symlink files.

# Dependencies
To specify dependencies, you need to add "deplist(Package manager)" list, in which you specify packages. I.e.: deplistPacman=(hyprland zsh) will tell sbpm to check for hyprland and zsh if your package manager is pacman. If your package manager or distro is not supported, open an issue and i will try to add it (or a pull request)

# Provides
This will specify where sbpm will link each file. You can have nothing to link, but you still need to create a list so that the script doesn't kill itself. The format is as follows: provides=("file1:directory1/file1" "file2:$HOME/.config/meow/file2")

# Setup
This is a function that will do whatever you put into it. For example, run additional scripts. You can also put nothing in there, just make sure that you have ":" symbol in there (essentially does nothing).

# File example
```
deplistPacman=(foot ttf-0xproto-nerd)

provides=("foot.ini:$HOME/.config/foot/foot.ini")

SETUP() { : }
```
This will check for foot and 0Xproto font and symlink foot.ini from repository root directory into user's .config/foot directory
