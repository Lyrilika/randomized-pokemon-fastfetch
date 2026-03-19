# Randomized Pokémon Fastfetch
<img width="2558" height="1438" alt="image" src="https://github.com/user-attachments/assets/df055446-3e9c-4727-96b4-e04adece8a27" />


This is my personal Fastfetch configuration, customized to fit my preferences. It uses [pokemon-colorscripts](https://gitlab.com/phoneybadger/pokemon-colorscripts) to display a random Pokémon sprite as the logo. Feel free to use this config as-is or modify anything to suit your own preferences.

This repository is mainly for my own personal use whenever I set up a new system, so I can easily reuse my Fastfetch configuration.

The guide here is also available for anyone who wants to add randomized Pokémon to their Fastfetch or use my config.

Keep in mind that this guide is **very simplified** and aimed at inexperienced users, so it may feel overly basic to some people.


# Dependencies
- fastfetch
- pokemon-colorscripts

## Installing dependencies

### Arch/Arch-based: 

```bash
sudo pacman -S fastfetch
yay -S pokemon-colorscripts-git
```
If you do not want to use an AUR helper you can also install [pokemon-colorscripts](https://gitlab.com/phoneybadger/pokemon-colorscripts) using this method:
```bash
git clone https://gitlab.com/phoneybadger/pokemon-colorscripts.git
cd pokemon-colorscripts
sudo ./install.sh
```
Optional (deleting the copied folder) (only do this if you used the second method to install pokemon colorscripts):
```bash
sudo rm -rf ~/pokemon-colorscripts
```

### Fedora 

```bash
sudo dnf install fastfetch git
git clone https://gitlab.com/phoneybadger/pokemon-colorscripts.git
cd pokemon-colorscripts
sudo ./install.sh
```
Optional (deleting the copied folder):
```bash
sudo rm -rf ~/pokemon-colorscripts
``` 
### Debian/Ubuntu

```bash
sudo apt install fastfetch git
git clone https://gitlab.com/phoneybadger/pokemon-colorscripts.git
cd pokemon-colorscripts
sudo ./install.sh
```
Optional (deleting the copied folder):
```bash
sudo rm -rf ~/pokemon-colorscripts
```

### OpenSUSE(Leap/Tumbleweed)
```bash
sudo zypper install fastfetch git
git clone https://gitlab.com/phoneybadger/pokemon-colorscripts.git
cd pokemon-colorscripts
sudo ./install.sh
```

Optional (deleting the copied folder):
```bash
sudo rm -rf ~/pokemon-colorscripts
```

### Other

simply install fastfetch using your distro's package manager if it isn't already installed, and install pokemoncolorscripts:
```bash
git clone https://gitlab.com/phoneybadger/pokemon-colorscripts.git
cd pokemon-colorscripts
sudo ./install.sh
```
Optional (deleting the copied folder):
```bash
sudo rm -rf ~/pokemon-colorscripts
```

### If you face any issues installing pokemon-colorscripts

Follow install instructions from the pokemon-colorscripts repo [here (github)](https://github.com/acxz/pokescript) [here (gitlab)](https://gitlab.com/phoneybadger/pokemon-colorscripts)

# Applying the config

## Using my own config

1. Download the `config.jsonc` file from the releases.

2. Move it to your Fastfetch config directory (`~/.config/fastfetch/`)

Note: if you do not have a fastfetch folder in your .config folder simply create the folder or generate a config by using the command below and replacing the generated config.jsonc with the one from this repo

```bash
fastfetch --gen-config
```

## Vanilla fastfetch with randomized pokemon (without my own config)

1. Download the `vanilla-config.jsonc` file from the releases.

2. Rename it to `config.jsonc` (Alternatively you can use `fastfetch --config path/to/vanilla-config.jsonc` to use that config without renaming it)

3. Move it to your Fastfetch config directory (`~/.config/fastfetch/`)

Note: if you do not have a fastfetch folder in your .config folder simply create the folder or generate a config by using the command below and replacing the generated config.jsonc with the one from this repo

```bash
fastfetch --gen-config
```

## Edit your own config

Add to/Edit to your config:
```bash
{"logo": {
        "type": "command-raw",
        "source": "pokemon-colorscripts --no-title --random"
        }}
```
