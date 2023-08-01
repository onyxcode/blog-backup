---
title: "How to Make Command Aliases in Bash"
datePublished: Mon Dec 07 2020 15:38:57 GMT+0000 (Coordinated Universal Time)
cuid: ckiepzig801au19s1c9u56wie
slug: bash-aliases
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1607355472049/txCpeXx73.jpeg
tags: tutorial, linux, terminal, bash, command-line

---

Hey all! This is a quick one, but I use command aliases all the time and they make my life *so much easier* when I'm in the terminal. Let's get started!


# 1. Opening the .bashrc file

The .bashrc file is short for "bash run commands". It can be located in your home directory at `~/.bashrc`. It contains a few preset configurations already. For this tutorial, I will be using Nano as my primary text editor. You can install it on Ubuntu and Debian using the command listed below.
```
sudo apt install nano -y
```

We can now cd to our home directory and run the listed below command to open our .bashrc file.

```
nano .bashrc
```

# 2. Adding aliases

I recommend putting aliases at the end of your .bashrc file. To get to the end of a file in Nano, press `Ctrl+V` repeatedly until you reach the end. Let's make a command alias for [asciinema](https://asciinema.org/). asciinema is a terminal recorder that I use often to capture command errors and demonstrate my Python scripts. I will call this alias `asc`, as the provided command, `asciinema` is quite lengthy. I will write the below listed code and explain it.

```
# Command aliases
alias asc='asciinema'
```

`alias` signals to Bash that the next word is a command alias. `asc` is the name of the alias. The `=` means the rest of the line defines the alias. `'asciinema'` defines the action that the alias carries out.

Now that we are done, save and close the file in Nano by typing `Ctrl+X`, `y`, and `Enter`.

# 3. Testing it out

Now let's see if our alias works. First, close your current bash session and open a new one. This reloads the .bashrc file with the new configuration.


```
onx@penguin:~$ asc rec
asciinema: recording asciicast to /tmp/tmpaliz0fko-ascii.cast
asciinema: press <ctrl-d> or type "exit" when you're done
onx@penguin:~$ echo hello world!
hello world!
onx@penguin:~$ echo awesome! it works!
awesome! it works!
onx@penguin:~$ exit
exit
asciinema: recording finished
asciinema: press <enter> to upload to asciinema.org, <ctrl-c> to save locally

View the recording at:

    https://asciinema.org/a/lPYgTBguPVz4g27KnuXO5pLTB
```

You can go view the recording for yourself if you like :)


# 4. You're done!

Congratulations! You've learned how to make command aliases in Bash! Have a great day everyone and let me know what I should write about next in the comments!