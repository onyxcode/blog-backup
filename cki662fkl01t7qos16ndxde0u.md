---
title: "An Introduction To The Apt Package Manager"
datePublished: Wed Oct 14 2020 08:55:28 GMT+0000 (Coordinated Universal Time)
cuid: cki662fkl01t7qos16ndxde0u
slug: apt-intro
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1606890651854/9Y4eVuaZn.jpeg

---

What is Apt? Apt is the default package manager on Ubuntu, a Linux distribution based on the popular Linux operating system, Debian. In this article we will be going over a couple basic features of Apt in order to give you, the user, a basic ability to install, uninstall and update packages.

## 1. Installing packages

Installing a package with Apt is pretty straightforward. First, you need the package name. Let’s use “sl” as an example. sl is a small Linux package that prints a moving steam locomotive across the screen when you type “sl” in the terminal. One thing to always remember. In most cases, unless you are logged in as “root”, you will need to type “sudo” before such a command, because it requires administrator privileges. With this information, to install a package, you need to type the following command:

```
sudo apt install sl
```

It should output something similar to this:

(Image on original post)


If it asks you if you wish to continue, press Y on your keyboard. Otherwise, if the output is similar to this, congratulations! You’ve successfully installed your first package with Apt! Type “sl” and press Enter to watch the steam locomotive go by. Choo choo!


> Tip

> Install multiple packages at once by adding a space between each package name.

## 2. Uninstalling packages

Uninstalling packages is just as easy as installing them. Instead of “install”, you simply replace it with “remove”. Let’s use our “sl” package from earlier as an example.

```
sudo apt remove sl
```

Your output should look something like this:

(Image on original post)

As before, if it asks you if you wish to continue, press Y on your keyboard. Otherwise, if the output is similar to this, congratulations! You’ve successfully removed a package with Apt!

## 3. Updating packages
With Apt, updating is a simple process, and it updates all installed packages at once. Simply run this command:

```
sudo apt full-upgrade
```

I won’t attach an image here because depending on how m
any packages you have installed, the output can get quite lengthy. However, it will most likely ask for confirmation, so press Y on your keyboard when prompted. full-upgrade checks all mirrors for the latest version of each package and installs it if the mirror’s version number is higher than your system’s.

## In conclusion
In this tutorial you learned you to install, uninstall and update packages with the Apt Package Manager. If you enjoyed this article, please comment and share!