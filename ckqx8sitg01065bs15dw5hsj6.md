---
title: "How to setup Starship Prompt and Zsh on Crostini"
datePublished: Sat Jul 10 2021 04:02:54 GMT+0000 (Coordinated Universal Time)
cuid: ckqx8sitg01065bs15dw5hsj6
slug: how-to-setup-starship-prompt-and-zsh-on-crostini
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1625889645384/wSQ3dALtXw.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1625889733556/-L530t4Q2.jpeg
tags: tutorial, linux, chrome, zsh, containers

---

Hey all! I made this guide after getting Starship successfully working on Bash, but zsh would refuse to accept the init script.

## Step 0 - Set a custom password
**This step is not required if you've already set a custom password for your Crostini container.**

Run `sudo passwd user`, where `user` is your username.


## Step 1 - Install zsh and setting as default shell
...whether it be from your package manager of choice, or [from source](https://github.com/zsh-users/zsh).

Then, simply run this command to add zsh's binary to `/etc/shells`:
`command -v zsh | sudo tee -a /etc/shells`

Now, set it as your default shell:
`chsh -s $(which zsh)`

## Step 2 - Install Starship Prompt

Run `curl -fsSL https://starship.rs/install.sh | bash` to start the installation. 

To add Starship's init script to your .zshrc file, simply run one last command:
`echo $(starship init zsh) >> ~/.zshrc`


## Congrats, you're done!

Enjoy your new beautiful and blazing fast prompt with the power of Rust and zsh!