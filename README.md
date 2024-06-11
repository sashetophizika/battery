# Battery

### Simple utility to monitor the battery in a stylish manner.

![image](screenshot.png "screenshot")
### Small version:

![image](screenshot_small.png "screenshot_small")
### Version with some extra options:

![image](screenshot_full.png "screenshot_full")

## Installation

```bash
git clone https://github.com/sasheto-phizika/battery.git
cp battery/battery ~/.local/bin # user installation
sudo cp battery/battery /usr/bin # system installation

```

## Usage

### Basic:
```
battery
```
### Options

* **-l**: monitor the battery live (close with `q` or `Esc`)
* **-s**: print a small inline battery instead
* **-f**: print a slightly thicker battery
* **-d**: print the current capacity as a number inside of the battery (does not work with -s)
* **-p=(printable)**: specify what to print with -d (c for capacity, p for power, t for temperature)
* **-m**: print minimal text output
* **-c**: use an alternate charging symbol (requires nerd fonts)
* **-n**: remove colors
* **-b=(bat_number)**: specify the battery number (default is the lowest one)

## Configuration

You can create `~/.config/battery/battery.conf` in order to change the colors and the default flags (the flags then become toggles that do the opposite).

### Default configuration:

```bash
#colors can be [red | green | yellow | blue | magenta | cyan | white | black | none] or a hex code with capital letters "#0000FF" 
color100p="green" #core color between 60-100%
color60p="yellow" #core color between 20-60%
color20p="red" #core color between 0-20%
color_shell="white" #color of the outer shell
color_charge="cyan" #color of the charging symbol
printable='c'

colors=true 
live=false 
minimal=false
small=false
digits=false
fat=false
alt_charge=false
```
The config file is just sourced as a bash script, so technically it can be used to run any code at the start and there has to be no whitespace between the equals signs. Be careful not to run random commands.
