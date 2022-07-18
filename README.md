# Awesome WM
Creating a collection of themes for the Linux Window Manager AwesomeWM

Changes to the bar are: 
- Removed the awesome logo
- Added CPU and RAM percentage widgets
- Separated date and time to separate widgets
- Replaced task list (windows open in current tag)with time widget

Some other changes:
- Terminal has been changed to alacritty instead
- Editor has been changed to Visual Studio code
- When you cursor ove a new window it focuses on that window has been removed
- Removed Titles of windows (titlebars_enabled = false)
- Changed close window (changed to: Super + "q")
- Added Browser shortcut(Super + "b")
- Tile is default layout instead of floating
# Usage

## Download
```bash
git clone -b master --depth=1 --single-branch https://github.com/luis-padilla-tech/awesomewm-themes.git
```
Once downloaded move rc.lua and/or theme folders to ~/.config/awesome

## Setup
If you are planning on only using the themes just copy the folders. Then change
```lua
beautiful.init(gears.filesystem.get_themes_dir().."default/theme.lua")
```
(or whatever code you have that manages themes) to 
```lua
beautiful.init(gears.filesystem.get_configuration_dir() .. "<theme folder name>/theme.lua")
```

# Dependencies

These are the required dependencies to run this particular setup. Feel free to change those in the "Other" secction in rc.lua or theme.lua

## Required

- awesome (the window manager)
- vicious (awesomewm widgets)
- dmenu (change thes default run prompt)

## Other
- alacritty (terminal in rc.lua)
- code (editor)
- firefox (browser in rc.lua)
- ttf-roboto-mono (font in theme.lua)

For my arch friends
```bash
$ sudo pacman -S awesome vicious code alacritty firefox ttf-roboto-mono
```