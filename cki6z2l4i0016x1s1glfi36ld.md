---
title: "Installation Methods for GitHub CLI"
datePublished: Wed Dec 02 2020 05:31:07 GMT+0000 (Coordinated Universal Time)
cuid: cki6z2l4i0016x1s1glfi36ld
slug: install-methods-gh-cli
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1606890708238/yJNU2lUKB.jpeg
tags: github, git, command-line

---

You can install GitHub CLI in quite a few ways, I will be going over each OS in this article.
# Windows
### WinGet
```
winget install gh
```
### scoop
```
scoop install gh
```
### Chocolatey
```
choco install gh
```
### MSI file
You can download the compiled MSI file from the [releases page](https://github.com/cli/cli/releases/latest).

<br>

# Linux
### (Debian/Ubuntu) apt
```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-key C99B11DEB97541F0
sudo apt-add-repository https://cli.github.com/packages
sudo apt update
sudo apt install gh
```
### (Fedora, CentOS, Red Hat Enterprise Linux) dnf
```
sudo dnf config-manager --add-repo https://cli.github.com/packages/rpm/gh-cli.repo
sudo dnf install gh
```
### (openSUSE Linux) zypper
```
sudo zypper addrepo https://cli.github.com/packages/rpm/gh-cli.repo
sudo zypper ref
sudo zypper install gh
```
### (Arch Linux) pacman
```
sudo pacman -S github-cli
```
### (Android) Termux
```
pkg install gh
```
### (Gentoo Linux) emerge
```
emerge -av github-cli
```
### (Kiss Linux) kiss
```
kiss b github-cli && kiss i github-cli
```
### snap
```
sudo snap install --edge gh && snap connect gh:ssh-keys
```
### (Nix/NixOS) nix
```
nix-env -iA nixos.gitAndTools.gh
```