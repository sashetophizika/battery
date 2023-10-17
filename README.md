# battery

Simple utility to check battery state that uses upower.
![image](screenshot.png "screenshot")

## Installation

```bash
git clone https://github.com/sasheto-phizika/battery.git
mv battery/battery ~/.local/bin # user installation
sudo mv battery/battery/ /usr/bin # system installaion

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
