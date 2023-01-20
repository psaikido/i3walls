# i3walls

Set groups of wallpapers as 'themes', one wallpaper for the first seven workspaces.  
Three random wallpapers for workspaces, 8, 9 & 10.

The program has two modes, one for using standalone and one for calling from a file manager like ranger, lf or similar.

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

Ranger and similar programs can choose a bunch of images in one go and then i3walls can be called to open them. When used this way the user gets the following menu:

- "add to existing theme?"
	Choose one of the defined themes to add the files to. More than 7 can be added but only the first 7 will be used.

- "add to new theme?"
	Choose a theme name and the files will be created

- "quit"


### Dependencies

[feh](https://wiki.archlinux.org/title/Feh)  
[sxiv](https://wiki.archlinux.org/title/Sxiv)

