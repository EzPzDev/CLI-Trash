# Super Simple Trash Command
A simple barebones cli command to trash a file or directory that *mostly* follows freedesktop guidelines. Trash pandas included!

<sub> By "mostly" it doesn't create a `$topdir/.Trash` directory or recognize seperate filesystems. So using it while in something like a NAS directory or flash drive will always move the trashed file/directory into your $home drive (`~/.local/share/Trash/`)

<sub> Only tested on OpenSUSE.

## Install
Download zip and copy trash to a `$PATH` directory or,

enter this command into your terminal:

```
curl -sSL "https://github.com/EzPzDev/Super-Simple-Trash-Command/raw/main/trash" -o ~/bin/trash
chmod +x ~/bin/trash
```
Add `~/bin` to your `$PATH` if it isn't already:
```
export PATH=$PATH:~/bin
```

## Usage
To use, simply type "trash [file/directory you want to trash]" into your terminal.

```
trash [file/directory to trash]
```

## Uninstall
Delete the file `trash` from `~/bin/` or wherever you copied it to.
