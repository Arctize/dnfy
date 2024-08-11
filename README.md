# dnfy

`dnfy` is a command-line tool that allows interactively searching and installing
packages using `dnf`, bringing the experience that
[paru](https://github.com/Morganamilo/paru) and
[yay](https://github.com/Jguer/yay) provide on Arch Linux to Fedora and other dnf-based distributions.

## Features

- Search packages and show more informative output than `dnf search`
    - Shows repository, package version, install size, and indicate if it's is
      already installed
- Interactively select packages to install from numbered search results

## Example
![image](https://github.com/user-attachments/assets/73ed0b23-1087-4318-a53b-acd5590cb2a2)

## Installation

Clone this repository (or download `dnfy` directly)
``` sh
git clone https://github.com/arctize/dnfy.git
cd dnfy
chmod +x dnfy # Make sure it's executable
```

Inside the directory where the file resides, it can be run directly with
`./dnfy`.

To make it runnable from anywhere, it needs to be in the `PATH`. Detailed
information on this can be found
[here](https://www.baeldung.com/linux/path-variable>).

A quick example:

``` sh
# Create bin dir for the local user
mkdir -p ~/.local/bin

# Create a link to dnfy in the git repo dir
ln -s $(pwd)/dnfy ~/.local/bin/dnfy

# Add the bin dir to PATH
# To add it permanently, add the line to ~/.profile or ~/.bashrc.
PATH=$PATH:$HOME/.local/bin
```
