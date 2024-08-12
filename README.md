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

Download `dnfy`:

```sh
curl -L -o dnfy https://raw.githubusercontent.com/arctize/dnfy/main/dnfy
chmod +x dnfy # Make sure it's executable
```

Move it to a location in PATH

```sh
sudo mv dnfy /usr/local/bin/
```

## Removal

```sh
sudo rm -f /usr/local/bin/dnfy
```