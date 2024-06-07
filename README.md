# CLI Trash Command
A simple cli command to trash a file or directory that *mostly* follows freedesktop guidelines. Trash pandas included!

<sub> By "mostly" it doesn't create a `$topdir/.Trash` directory or recognize seperate filesystems. So using it while in something like a NAS directory or flash drive will always move the trashed file/directory into your $home drive (`~/.local/share/Trash/`)

<sub> Tested on OpenSUSE and Debian.

## Install
Download zip and copy trash & resources to a `$PATH` directory or,

enter this command into your terminal:

```
curl -sSL "https://github.com/EzPzDev/Super-Simple-Trash-Command/raw/main/trash" --create-dirs -o ~/bin/trash
curl -sSL "https://github.com/EzPzDev/Super-Simple-Trash-Command/raw/main/resources/tput-colors" --create-dirs -o ~/bin/resources/tput-colors
curl -sSL "https://github.com/EzPzDev/Super-Simple-Trash-Command/raw/main/resources/help" --create-dirs -o ~/bin/resources/help

chmod +x ~/bin/trash
```
Add `~/bin` to your `$PATH` if it isn't already:
```
export PATH=$PATH:~/bin
```

## Usage
To use, simply type "trash [file/directory you want to trash]" into your terminal.
```
trash [option] [file/directory]
```

## Uninstall
Delete the file `trash` and `resources` from `~/bin/` or wherever you copied it to.
