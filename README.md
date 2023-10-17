# battery

Simple utility to check battery state that uses upower

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

To stay and monitor live:
```
battery -l
```
To escape live view press `q` or `Ecs`. 


For minimalistic text output:
```
battery -m
```
The `-m` flag overwrites all other ones.
