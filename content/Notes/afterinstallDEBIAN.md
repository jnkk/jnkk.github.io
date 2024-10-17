---
title: Steps after installing Debian 12
tags: index
---


# This is for Debian 12, if another reinstall is needed

## change sourcelist. make a backup of the original file and copy and paste in /etc/apt 

> [!]IMPORTANT
> Make sure to backup first and then edit the files

```txt
deb http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware  
deb-src http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware  

deb http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware  
deb-src http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware  

deb http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware  
deb-src http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware  
```

## post debian 12 install to download

```bash
sudo apt install curl wget git micro btop build-essential cmake gcc brew vscodium nvidia-tesla-470-driver npm nodejs
```  

> [!]NOTE
> current setup is using a dell laptop that has a old nvidia  
> use-> nvidia-tesla-470-driver  
> nvidia-detect

## Install homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Setup XDG BASE DIR

```bash
export XDG_CONFIG_HOME="$HOME/.config"
export XDG_DATA_HOME="$HOME/.local/share"
export XDG_CACHE_HOME="$HOME/.cache"
export XDG_STATE_HOME="$HOME/.local/state"

```

### Install [xdg-ninja](https://github.com/b3nj5m1n/xdg-ninja)

> []NOTE:
> This is after installing the xdg-ninja

```bash
export RUFF_CACHE_DIR="$XDG_CACHE_HOME/ruff"
export RUSTUP_HOME="$XDG_DATA_HOME"/rustup
export CARGO_HOME="$XDG_DATA_HOME"/cargo
export GNUPGHOME="$XDG_DATA_HOME"/gnupg
```

## How to download and make use of personal notes

1. set your git username and email

```bash
git config --global user.name "<yourusername>"
git config --global user.email "<youruseremail>"
```

2. create ssh-key

```bash
ssh-keygen -t rsa
```

> [!]NOTE  
> using SUDO goes to the root user.

3. add ssh key to [github](https://github.com/settings/keys)  

4. download the GIT version and not the https. so the git push command works.


## other must to install not with apt

go rust cloudflare-warp speedtest-cli fast-cli ollama

## apps using BREW  

lazygit ruff npm nodejs

## Install [NERDFONTS](https://github.com/ryanoasis/nerd-fonts)

Jetbrains

## install miniconda for shell-gpt

[miniconda](https://docs.anaconda.com/miniconda/miniconda-install/)  
Make sure to download sh their file. use bash command to install those.
last time I tried their failed because of the agreements.

[Shell-gpt guide](https://github.com/TheR1D/shell_gpt/wiki/Ollama) is here

Run this if [shell-gpt](https://github.com/TheR1D/shell_gpt) is installed globally

```bash
git diff | sgpt "Generate git commit message, for my changes"
```

takes over 10 seconds with current setup. OLD LAPTOP.

## best terminal by far is [FISH](https://fishshell.com/)
have to learn it.
if fish is set up. type this:

```fish
fish_config theme choose Tomorrow
```

## tutorial for installing QEMU/KVM
[youtube](https://www.youtube.com/watch?v=GgAQw08zJzs)
or go to [chatgpt](https://chatgpt.com/)/[perplexity](https://www.perplexity.ai/)

"how to install qemu/kvm on debian 12"
