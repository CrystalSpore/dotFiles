# DotFile collection repo
Uses gnu `stow` for config management. This repo is just the collection of config files

## Prerequisite programs
- stow: `sudo apt install stow`
- git: `sudo apt install git`

## Instructions for use:

### Setting up for a new system:
In home directory, run the below commands
```
git clone git@github.com:CrystalSpore/dotFiles.git
cd dotFiles
./run_stow.sh
cd ~
```

### Adding a new program's config files:
Create a new directory, the same as the program/package name. This will be the same as the argument for `stow <directory_name>`. Copy/Move over the config files for the program from the `$HOME` or `$XDG_CONFIG` directory into this directory, & then run the `stow` command.


## What about your accidental re-creation of the `stow` program? What's the best way to see that?
If you go to [this commit](https://github.com/CrystalSpore/dotFiles/tree/e102a91e7b03a8bff1cea3c4cdab5a043575bdbb), you can browse the file system & install script from that point in time.
