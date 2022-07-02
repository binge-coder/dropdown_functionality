# README.md
make any terminal behave like quake/guake/yakuake through using this


### <a name="dependencies"> You need the following programs to make it work (dependencies) </a>
1. sxhkd ( https://github.com/baskerville/sxhkd )
2. tdrop ( https://github.com/noctuid/tdrop )
3. wmctrl (install from apt ```sudo apt install wmctrl```)

[Note : make sure to have the dependencies of the above programs as well... i.e. dependencies of dependencies, can be found on their github pages]

### Operating systems:
1. Linux -> should work
2. MacOs -> not tested, dependencies probably not available
3. Windows -> this solution will not work... try looking somewhere else

### tested on:
1. linux mint 20.3 (DE:Cinnamon) (WM:Mutter)
{i.e. the default cinnamon desktop in linux mint}		
**WORKING**
[Note : should work in all desktop env in linux mint and ubuntu]

## Procedure
1. Install dependencies [dependencies](#dependencies) .
2. git clone this repository 
`git clone https://github.com/binge-coder/dropdown_functionality.git ~/dropdown_files`
3. Copy sxhkd folder from cloned repo to ~/.config/ 
`cp -r ~/dropdown_files/sxhkd ~/.config/ `
4. make changes to sxhkdrc as per your use case
### changes


	