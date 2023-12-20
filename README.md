# Battery

Simple utility to check battery state that uses upower.
![image](screenshot.png "screenshot")

## Installation

```bash
git clone https://github.com/sasheto-phizika/battery.git
cp battery/battery ~/.local/bin # user installation
sudo cp battery/battery /usr/bin # system installation

```

## Usage

Basic:
```
battery
```
To stay and monitor live (`q` or `Ecs` to exit):
```
battery -l
```
For a small inline battery (also works with `-l` and might not print properly in a `tty`):
```
battery -s
```

For minimalistic text output:
```
battery -m
```
The `-m` flag overwrites flags above.


If you want to change the colors, modify the top of the script using ANSI escape codes (`\033[38;2;R;G;Bm` format for terminals with true color support).

To remove colors:
```
battery -n
```

To specify the battery:
```
battery -b BAT_NUMBER
```
The default is the one with the smallest number found in `/sys/class/power_supply/` (usually 0, equivalent to `-b 0`).
