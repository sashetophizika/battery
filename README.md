# Battery

Simple utility to check battery state that uses upower.
![image](screenshot.png "screenshot")

## Installation

Dependencies:\
[upower](https://gitlab.freedesktop.org/upower/upower) (Tested on version 1.90.2-1), which could be found in most distro repositories 


```bash
git clone https://github.com/sasheto-phizika/battery.git
cp battery/battery ~/.local/bin # user installation
sudo cp battery/battery/ /usr/bin # system installaion

```

## Usage

Basic:
```
battery
```

With colors:
```
battery -c
```
If you want to change the colors, modify the top of the script using ANSI escape codes (`\033[38;2;R;G;Bm` format for terminals with true color support).

To stay and monitor live (`q` or `Ecs` to exit):
```
battery -l
```
For a small inline battery (does not work with `-l`):
```
battery -s
```

For minimalistic text output:
```
battery -m
```
The `-m` flag overwrites all other ones.
