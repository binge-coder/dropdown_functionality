# README.md
make any terminal behave like quake/guake/yakuake (i.e. have a drop down feature) using this


### <a name="dependencies"> You need the following programs to make it work (dependencies) </a>
1. sxhkd ( https://github.com/baskerville/sxhkd )
2. tdrop ( https://github.com/noctuid/tdrop )
3. wmctrl ( install from apt ```sudo apt install wmctrl``` or see this https://archlinux.org/packages/community/x86_64/wmctrl/ or see this http://tripie.sweb.cz/utils/wmctrl/ )

[Note : make sure to have the dependencies of the above programs as well... i.e. dependencies of dependencies, can be found on their github pages]

### Operating systems:
1. Linux -> should work
2. MacOs -> not tested, dependencies probably not available
3. Windows -> this solution will not work... try looking somewhere else

### tested on:
1. linux mint 20.3 (DE:Cinnamon) (WM:Mutter)
{i.e. the default cinnamon desktop in linux mint} ->**WORKING**
[Note : should work in ubuntu as well]

## Procedure
1. Install the 3 dependencies [from above](#dependencies) .
2. git clone this repository 
```
git clone https://github.com/binge-coder/dropdown_functionality.git ~/dropdown_files
```

3. Copy sxhkd folder from cloned repo to ~/.config/   or use this in terminal  :
```
cp -r ~/dropdown_files/sxhkd ~/.config/ 
```

4. go to the file or use this in terminal : 
```
xdg-open ~/.config/sxhkd
``` 
5. make changes to sxhkdrc as per your use case see. open the sxhkdrc file and read the instructions. 
6. see for valid keybindings and format of skhkdrc: https://github.com/baskerville/sxhkd/blob/master/doc/sxhkd.1.asciidoc#configuration
7. **Last very important step - have sxhkd run on startup. see below**

### start automatically on startup
1. search for keywords like "startup" or "auto" in your system settings.
2. A relevant setting will open where you need to add a custom command to the list of startup applications and commands.
3. Give the command a relevant title and put sxhkd as the command.
4. Done. Make sure to use "pkill -USR1 -x sxhkd" in terminal to refresh sxhkd. you may need to log out and log in perhaps   

* you can remove the cloned folder now or use this in terminal : 
```
rm -r -f ~/dropdown_files
```
