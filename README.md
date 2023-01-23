# i3walls

Set groups of wallpapers as 'themes', one wallpaper for each of ten workspaces on [i3wm](https://i3wm.org/).  
This is a bash script so will only work in *nix environments.  

![i3demo-3](https://user-images.githubusercontent.com/208479/214102327-d620f66c-8440-4125-af0c-3265f299b1a9.gif)

## Setup

`git clone https://github.com/psaikido/i3walls`  
cd into the new directory  
`chmod +x i3walls`  
`chmod +x setup`  
`./setup`

It creates a directory ~/.config/i3/i3walls which will contain a default theme. The wallpapers are from https://gitlab.com/dwt1/wallpapers.  

The existing ~/.config/i3/config file is updated to add a function and symlinks so that the program feh updates each workspace's background.

The program has two modes, one for using standalone and one for calling from a file manager like ranger, lf, fzf or similar.

## Standalone

Invoking 'i3walls' from the command line gives the following functions:

- "show current wallpapers"
	The sxiv file viewer displays thumbnails of the current wallpapers

- "set theme"
	Choose from a list of themes and set one as the current theme

- "edit a theme"
	Open the theme file in an editor to manage manually

- "show themes"
	Show the themes that have been defined

- "new theme"
	Create a new theme. Choose a name and then get some wallpapers for it

- "quit"

## File Manager

i3walls can be given one or many file paths as arguments eg: 
	`i3walls ~/wallpapers/wall.jpg`

Ranger and similar programs can choose a bunch of images in one go and then i3walls can be called to open them. In ranger, select the files, press 'r' and type 'i3walls' in the 'open_with' dialog. When used this way the user gets the following menu:

- "add to existing theme?"
	Choose one of the defined themes to add the files to.

- "add to new theme?"
	Choose a theme name and the files will be created

- "quit"


### Dependencies

[i3wm](https://i3wm.org/)  
[gum](https://github.com/charmbracelet/gum)  
[feh](https://wiki.archlinux.org/title/Feh)  
[sxiv](https://wiki.archlinux.org/title/Sxiv)

