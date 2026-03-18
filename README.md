# Randomized Pokémon Fastfetch
<img width="2558" height="1438" alt="image" src="https://github.com/user-attachments/assets/df055446-3e9c-4727-96b4-e04adece8a27" />


This is my personal Fastfetch configuration, customized to fit my workflow and aesthetic preferences. It uses [pokemon-colorscripts](https://gitlab.com/phoneybadger/pokemon-colorscripts) to display a random Pokémon sprite as the logo. Feel free to use this config as-is or modify anything to suit your own setup.

# Dependencies
- fastfetch
- pokemon-colorscripts

## Installing dependencies

Arch/Arch-based: 

  ```bash
sudo pacman -S fastfetch
yay -S pokemon-colorscripts
```
# Applying the config

1. Download the `config.jsonc` file from this repository.

2. Move it to your Fastfetch config directory ('~/.config/fastfetch/')

Note: if you do not have a fastfetch folder in your .config folder simply create it and put the .jsonc inside or generate a config by using the command below and replacing the generated config.jsonc with the one from this repo

```bash
fastfetch --gen-config
```
