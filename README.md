# altline

[![License](https://img.shields.io/github/license/pangteypiyush/altline.svg)](https://raw.githubusercontent.com/pangteypiyush/altline/master/LICENSE) [![Last Commit](https://img.shields.io/github/last-commit/pangteypiyush/altline.svg)](https://github.com/pangteypiyush/altline/commits)

A dirty powerline alternative.

## Usage

Recommended font [NerdFonts](https://github.com/ryanoasis/nerd-fonts)

```sh
# default
echo 'source /usr/share/bash-altline/altline && al_zen' >> ~/.bashrc

# zen
echo 'source /usr/share/bash-altline/altline && al_default' >> ~/.bashrc
```

## Customization

```sh
# download default theme source
curl https://raw.githubusercontent.com/pangteypiyush/altline/master/themes_src/default.ini -o ~/.custom.ini

# build theme
mktheme ~/.custom.ini ~/.custom

# source custom theme in bashrc
source ~/.custom && al_default
```

## Default

Context

![context](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/context-default-1.png)

Home

![home](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/home-default-1.png)

Root

![root](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/root-default-1.png)

## Zen

Context

![context](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/context-1.png)

Home

![home](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/home-1.png)

Root

![root](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/root-1.png)

## Themes

Default

![default](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/default-1.png)

Onyx

![onyx](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/onyx-1.png)

Onyx arrow

![onyxarrow](https://raw.githubusercontent.com/pangteypiyush/altline/screenshot/onyx_arrow-1.png)
