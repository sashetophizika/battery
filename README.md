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
* **-m**: print minimal text output
* **-c**: use an alternate charging symbol (requires nerd fonts)
* **-n**: remove colors
* **-b=(bat_number)**: specify the battery number (default is the lowest one)

## Configuration

You can create `~/.config/battery/battery.conf` in order to change the colors and the default flags (the flags then become toggles that do the opposite).

### Default configuration:

```bash
color100p="\033[0;32m" #core color between 60-100%
color60p="\033[0;33m" #core color between 20-60%
color20p="\033[0;31m" #core color between 0-20%
color_shell="\033[0m" #color of the outer shell
color_charge="\033[0;36m" #color of the charging symbol

colors=true 
live=false 
minimal=false
small=false
digits=false
fat=false
alt_charge=false
```

