---
title: "How to install palera1n on a Chromebook"
datePublished: Sun Jul 02 2023 23:18:36 GMT+0000 (Coordinated Universal Time)
cuid: cljm1zt3t000009l29fkbgzug
slug: how-to-install-palera1n-on-a-chromebook
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1688339800538/c7c71565-19ab-4808-b3ee-19cadede027e.jpeg
tags: ios, hacking, exploit, palera1n

---

## Notes and Warnings

* If you have a Chromebook with a Ryzen processor, this process has a much lower success rate. If possible, use a different computer or if you must, a Chromebook with an Intel processor.
    
* If you're using a USB-C to Lightning cable for this process, there's a chance you'll face some trouble getting into DFU mode. If that happens, get yourself a USB-A to Lightning cable and, if needed, grab a USB-C to USB-A adapter as well.
    
* You ***must*** enable Developer Mode on your Chromebook for this process to work.
    

## **Getting What You Need**

1. All you need is to download the latest release of [**palera1n**](https://github.com/palera1n/palera1n/releases/latest).
    

## **Allowing palera1n to Run**

1. Time to get the palera1n binary in the right place. Move the downloaded file to `/usr/local/bin`.
    
    * Here's what you need to do:
        
        * Press `Ctrl` + `Alt` + `T` to open the terminal.
            
        * Type in `shell`.
            
        * Run the command `mv ~/Downloads/palera1n-linux-* /usr/local/bin/`.
            
2. Now, in the terminal, run the command `sudo mount -o remount,exec /tmp`. You'll need to do this every time you reboot your Chromebook.
    
3. Whenever you're ready to jailbreak, make sure your device is connected and manually enter Recovery Mode. You can easily find instructions on how to do this with a quick Google search.
    

## **Running palera1n**

1. Open the terminal and execute the `palera1n` binary using `TERM=linux sudo palera1n`. If the binary doesn't work, you might need to run `sudo chmod a+x /usr/local/bin/palera1n`.
    
2. After this, palera1n should automatically detect your device in Recovery Mode and ask you to press Enter.
    
3. Follow the instructions to put your device into DFU mode.
    
4. As soon as you see the Apple logo on your device, unplug it, and then plug it back in. This will allow your Chromebook to detect the PongoOS USB device.
    

Just remember, it's an experimental process, so be prepared for any unexpected bumps along the way.