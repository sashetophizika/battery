# Battery

Simple utility to check battery state that uses upower.
![image](screenshot.png "screenshot")

## Installation

Dependencies:\
[upower](https://gitlab.freedesktop.org/upower/upower)(Tested on version 1.90.2-1)


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

To stay and monitor live (`q` or `Ecs` to exit):
```
battery -l
```

For minimalistic text output:
```
battery -m
```
The `-m` flag overwrites all other ones.
